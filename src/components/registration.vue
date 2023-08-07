<script>
export default {
    name: "registration",
    data() {
        return {
            login: '',
            password: '',
        }
    },
    methods: {
        onSubmit(){
            //alert('Отправка формы')
            this.handlerRegistration(
                this.login,
                this.password
            )
        }
    },
    props: ['handlerRegistration', 'error', 'swither']
}
</script>

<template>
<div class="container">
  <div class="form">
    <h1>Регистрация</h1>
    <form v-on:submit.prevent="onSubmit">
        <input v-model='login' placeholder="Введите логин" name="login" class='login' type="text" />
        <input v-model='password' placeholder="Введите пароль" name="passord" class='password' type="password" />
        <input type="submit" class='enter' value='Зарегестрироваться' />
        {{this.error}}
    </form>
    <div class='button-container'>
        <div class='button-container'>
        <button @click="swither('auth')">
            Авторизация
        </button>
        <button @click="swither('reg')" class='is-active'>
            Регистрация
        </button>
    </div>
    </div>
  </div>
 </div>
</template>

<style scoped>
.is-active{
    outline: 1px solid red;
}
.container {
    background-color: rgba(255,255,255, 0.4);
    height: 100vh;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    background-image: url(../../public/assets/theme/3.jpeg);
}
.form {
    background-color: rgba(4, 4, 4, 0.532);
    width: 600px;
    height: 600px;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
}
.form h1{
    text-align: center;
    width: 100%;
    color: white;
}
form {
    padding: 55px;
    background: white;
    text-align: center;
}

input {
    width: 80%;
    height: 50px;
    margin: 15px;
}

.login{

}

.password{

}

.enter{

}
</style>