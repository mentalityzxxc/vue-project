<script>
import Board from './components/board.vue'
import Login from './components/login.vue'
import Registration from './components/registration.vue'

export default {
    name: "App",
    data() {
      return {
        isAuth: 'auth',
        error: undefined,
        userData: null,
        users: [
          {
            login: 'admin',
            password: 'admin',
            avatar: 'https://cdn-icons-png.flaticon.com/512/5556/5556468.png'
          },
          {
            login: 'user1',
            password: 'user1',
            avatar: 'https://cdn-icons-png.flaticon.com/512/5556/5556468.png'
          },
          {
            login: 'user2',
            password: 'user2',
            avatar: 'https://static.vecteezy.com/system/resources/previews/009/397/892/original/woman-face-expression-clipart-design-illustration-free-png.png'
          }
        ]
      }
    },
    methods: {
      switchDisplay(display){
        this.isAuth = display;
      },
      login(login, password){
        console.log('Авторизация');
        //Получить в методу, введенный пользователем логин и пароль
         console.log(login, password, this);
         // Ищем по введенному логину и паролю пользьзователя
         const component = this;
         const user = this.users.find(function(user){
            //Условие нахождения пользователя в массиве
            //Пароль и логин, должны подходить по условию, как минимум в одном объекте
            if(user.login == login && user.password == password){
                //isAuth - нужно изменить на true
                console.log(component)
                //component.isAuth = true;
                return user
            }
         })
         if (user) {
            //При успешном нахождении пользователя
            // 1 - возвращаем состояние ошибки в исходное
            // 2 - меняем флаг isAuth, который влияет на отображение определенного компонента
            // 3 - запишем данные пользователя для передачи в компонент board
            component.error = undefined
            component.isAuth = 'end';
            component.userData = user
         } else {
            component.error = 'Пользователь не найден';
         }
      },
      registration(login, password){
        console.log(`registration: ${login}, ${password}`);
        //Проверяем, не существуюет ли уже, аналогичного пользователя в базе данных
        const searchUserInDB = this.users.find(function(user) {
          //Метод find, по аналогии с forEach перебирает все эдлементы массива users в компоненте
          // Если находит совпадение с пользователем в массиве и логином введенным с формы, тогда возвращается найденный пользователь
          if(user.login == login) {
            return user
          }
        });

        if (searchUserInDB) {
            //Если пользователь нашелся в базе, выводим ошибку
             this.error = 'Пользователь с таким логином уже есть в системе';
        } else {
          //Если такого логина нет, нужно закончить регистрацию
          //Создадим объект пользователя, который добави в базу данных
          let user = {
            login: login,
            password: password
          }
          //Обновим базу данных, запушив объект пользователя в общий масиив с пользователями
          this.users.push(user)

          //Производим авторизацию в приложении
          this.error = undefined
          this.isAuth = 'end';
          this.userData = user

        }
      },
      logout(){
          this.isAuth = 'auth';
          this.userData = null
      }
    },
    components:{
      Board,
      Login,
      Registration
    }
}
</script>

<template>
  <Login :handlerLogin='login' :error="error" v-if="isAuth === 'auth'" :swither="switchDisplay" />
  <Registration :handlerRegistration='registration' v-else-if="isAuth === 'reg'" :swither="switchDisplay"/>
  <Board :user="userData" :logout="logout" v-else-if="isAuth === 'end'" />
  <div v-if="error" class="error">{{error}}</div>
</template>

<style scoped>
.error {
  position: absolute;
  top: 10px;
  right: 10px;
  font-size: 24px;
  color: red;
}
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
