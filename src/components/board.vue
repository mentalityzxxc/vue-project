<script>
    import BoardColumn from './board-column.vue'
    export default {
        'name': "Board",
        data() {
            return {
              boards: {

              },
              wallpaper: [
                "https://klevtsovaelena.github.io/wallpaper/img/BlackWhite1.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/BlackWhite2.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/BlackWhite3.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/BlackWhite4.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/BlackWhite5.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/BlackWhite6.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/BlackWhite7.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/BlackWhite8.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/BlackWhite9.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/BlackWhite10.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/BlackWhite11.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/BlackWhite12.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/1.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/2.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/3.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/4.png",
                "https://klevtsovaelena.github.io/wallpaper/img/5.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/6.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/7.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/8.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/9.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/10.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/11.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/12.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Shine1.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Shine2.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Shine3.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Shine4.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Shine5.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Shine6.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Shine7.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Shine8.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Shine9.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Shine10.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Shine11.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Shine12.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Winter1.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Winter2.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Winter3.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Winter4.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Winter5.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Winter6.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Winter7.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Winter8.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Winter9.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Winter10.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Winter11.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Winter12.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Fire1.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Fire2.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Fire3.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Fire4.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Fire5.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Fire6.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Fire7.jpeg",
                "https://klevtsovaelena.github.io/wallpaper/img/Fire8.png",
                "https://klevtsovaelena.github.io/wallpaper/img/Fire9.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Fire10.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Fire11.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Fire12.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Flower1.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Flower2.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Flower3.jpeg",
                "https://klevtsovaelena.github.io/wallpaper/img/Flower4.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Flower5.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Flower6.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Flower7.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Flower8.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Flower9.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Flower10.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Flower11.jpg",
                "https://klevtsovaelena.github.io/wallpaper/img/Flower12.jpg",
              ],
              currentWallpaper: 0,
              activeMenu: false,
              list: [
                {
                  id: '1',
                  title: 'Купить доски',
                  checked: true,
                },
                {
                  id: '2',
                  title: 'Нанять строителей',
                  checked: false,
                },
                {
                  id: '3',
                  title: 'Заплатить за аренду',
                  checked: true,
                },
              ],
              inprogress: [
                {
                  id: '4',
                  title: 'Закупить инструменты',
                  checked: true,
                },
              ],
              done: [
                {
                  id: '5',
                  title: 'Рассчитать денежные средства',
                  checked: true,
                },
              ],
              newTask: null,
            };
        },
        props: ['test', 'user', 'logout'],
        methods: { 
          handlerDragend(event, type){
            console.log('handlerDragend');
            //console.log(event.target.getAttribute('id'));
            //Получить элемент (колонку) на которую нужно переместить задачу
            //elementFromPoint - Функция из чистого JS, для получения его по его координатам.
            //https://developer.mozilla.org/en-US/docs/Web/API/Document/elementFromPoint
            let Element = document.elementFromPoint(event.x, event.y);
            console.log(Element);
            //Условие, при котором мы перехватываеем, момент, 
            //когда пользователь отпускает задачу в верхний белый блок с рукой
            // Отпускаем элемент именно над блоком с классом drop-zone
            if(Element.getAttribute('class') == 'drop-zone'){
                console.log('Элемент опустился над drop-zone')
                //Найти тот самый элемент, который я перетаскиваю
                // 1 - Из Ивента, получим идентификатор элемента
                const id = event.target.getAttribute('id')
                // 2 - Найти элемент из конкретного массива
                // 2.1 - получить массив (list, inprogress или done) в переменную из которого мы перетаскиваем задачу
                let arrayFrom = this[type];
                // 2.2 - Найти в том массиве, задачу которую мы перетаскиваем
                let element = arrayFrom.find(el => el.id == id);
                console.log('element',element)
                // 2.3 - удалить элемент, из массива, из столбца которого мы перетаскиваем
                //Получаем новый отфильтрованный массив, со всеми элементами, кроме того, что мы перетаскиваем
                let filteredNewArray = arrayFrom.filter(el => el.id !== id);
                //Перезаписываем массив из которого удалили элемент
                this[type] = filteredNewArray
                console.log('filteredNewArray',filteredNewArray)
                //Получим имя массива, в который перемещаем задачи
                let arrayTo = Element.getAttribute('name');
                console.log('arrayTo', arrayTo)
                //Получить массив в который переносим элемент и поместим элемент в его начало
                //unshift - функция для добавление элемента в начало массива, противоположность функции push
                this[arrayTo].unshift(element);
            }
          },
          changeBackground(number){
            this.currentWallpaper = number;
            //Принудительно закрываем Меню
            this.activeMenu = false;
          },
          openCloseMenu(){
            //alert('Сработала функция openCloseMenu')
            //Проверить открыто или закрыто сейчас Меню
            if (this.activeMenu) {
              //если перменная в значении true, то меняем на false
              this.activeMenu = false;
            } else {
              //если перменная в значении false, то меняем на true
              this.activeMenu = true;
            }
          },
          addTask(task, columnName){
            //Готовим объект с задачей
            const taskObject = {
              id: Math.random(),
              title: task
            }
            //Пушим в определенную колонку
            this[columnName].push(taskObject)
          },
          delTask(idTask, columnName){
            //Найти в нежной колонке, данные и отфильтровать их таким образом, чтобы удаляемая задача не появилась на интрфейсе
            this
            columnName

            const newDataInColumn = this[columnName].filter( function(task) {
              console.log('task',task)
              //Если идентификатор, задачи, которую мы перебираем в цикле с помощью функции filter, НЕ равен, ID удаляемой задачи
              if(idTask !== task.id) {
                //То возвращаем этот элемент в новый массив
                return task
              }
            })
            console.log('Новые данные', newDataInColumn)
            //Перезапишем данные на полученные из предыдущего шага
            this[columnName] = newDataInColumn;
          },
          editTask(idTask, columnName){
            //Найдем старый заголовок задачи 
            //Декомпозируем нужное поле объекта
            const { title } = this[columnName].find(function(task){
                //Ищем задачу по передаваемому идентификатору
                if(task.id == idTask) {
                  return task; 
                }
            })
            console.log(title)
            const newTitle = prompt('Введите новое название задачи', title);
            //Перебираем еще раз колонку задач для редактирования
            
            //Предварительно, создадим новый массив для обновленных данных
            let newArray = [];
            //Перебираем выбранную колнку с задачами
            this[columnName].forEach(function(task, index){
                //Ищем задачу по передаваемому идентификатору
                //Создаем новый объект для нового массива на каждом повторении цикла
                //Создаю НОВЫЙ пустой объект и далее заполяю его
                let objectTask = {}
                //Записываю в поле ID идентификатор перебираемоей задачи
                objectTask.id = task.id;
                //Если идентификатор, совпал с тем, что я передал из параметра метода, то я в новый объект, записываю новый заголовок
                if(task.id == idTask){
                  //Так не сработало обновление интерфейса!
                  //this[columnName][index].title = newTitle
                  objectTask.title = newTitle;
                }else{
                  //Если условие не прошло оставляем старый заголовок
                  objectTask.title = task.title;
                }

                /* 
                Усложненный пример (аналог)
                let task = {
                  id: task.id,
                  title: task.id == idTask ? newTitle : task.title
                }
                */

               //Запушить в новый массив новый объект
               //Эдентичные по своей задаче записи
               //Обе добавляют объекты в массив
               //newArray[index] = task
               newArray.push(objectTask)
            })
            //Заменяем существующий массив колонки с задачами на новый, обработаный
            this[columnName] = newArray
          }
        },
        //Регистрируем внешний компонент внутри родительского
        components: {
            'board-column': BoardColumn
        }
    }
</script>

<template>
  <div>
    <div class='board' :style="{'background-image': `url(${wallpaper[currentWallpaper]})` }"> 

      <button class='board__button-change-theme' @click='openCloseMenu'>
         <img :src='wallpaper[currentWallpaper]' />
         Сменить фон
      </button>
      
      <div class='user-block' v-if='this.user'>
        <div class='avatar'>
            <img :src="this.user.avatar" :alt="this.user.login">
        </div>
        <div class='login'>
          {{this.user.login}}
        </div>
        <button @click="logout">
          Выйти
        </button>
      </div>

      <div :class="[activeMenu ? 'board__theme-wrapper board__theme-wrapper--active' : 'board__theme-wrapper']">
          <div id='wallpapers'>
            <div 
              v-for="(item, index) in wallpaper"
              class='wallpapers__item'
              :key="index"
              :style="{'background-image': `url(${item})` }"
              @click='changeBackground(index)'
            >
            </div>
          </div>
          <div class='close-wallpapers' @click='openCloseMenu'>
              {{'<'}}
          </div>
      </div>
      <board-column 
        :delTask="delTask" 
        :addTask="addTask" 
        :editTask="editTask" 
        :taskModel="newTask" 
        title='На складе' 
        :items="list" 
        name='list' 
        :handlerDragend='handlerDragend'
      ></board-column>
      <board-column 
        :delTask="delTask" 
        :addTask="addTask" 
        :editTask="editTask" 
        :taskModel="newTask" 
        title='У курьера' 
        :items="inprogress" 
        name='inprogress' 
        :handlerDragend='handlerDragend'
      >
      </board-column>
      <board-column 
        :delTask="delTask" 
        :addTask="addTask" 
        :editTask="editTask" 
        :taskModel="newTask" 
        title='Доставлено' 
        :items="done" 
        name='done' 
        :handlerDragend='handlerDragend'
      >
      </board-column>
    </div>
  </div>
</template>

<style scoped>
  .user-block{
    background: white;
    position: absolute;
    bottom: 0;
    right: 0;
    color: black;
    width: 200px;
    display: flex;
    align-items: center;
    z-index: 2;
    padding: 5px;
  }
  .avatar{
    height: 100px;
  }
  .user-block img{
     height: 100%;
  }
  .close-wallpapers{
    display: flex;
    position: fixed;
    top:0;
    height: 100vh;
    width: 35px;
    justify-content: center;
    align-items: center;
    color: black;
    background-color: rgba(255, 255, 255, 0.9);
  }
  .board{
      height: 100%; 
      display: flex;
      justify-content: center;
      position: absolute;
      width: 100%;
      left: 0;
      top: 0;
  }
  .wallpapers__item {
      display: inline-block;
      position: relative;
      width: 160px;
      height: 90px;
      background-size: cover;
      margin: 7px;
      border-radius: 0 20px;
      overflow: hidden;
      transition: all 0.5s;
      cursor: pointer;
  }
  .board__theme-wrapper {
      position: fixed;
      display: flex;
      justify-content: end;
      width: 400px;
      height: 100vh;
      background-color: rgba(255, 255, 255, 0.7);
      z-index: 2;
      top: 0;
      left: -400px;
      overflow-y: scroll;
      transition: all 0.4s;
  }
  .board__theme-wrapper--active{
    left: 0px;
  }
  .board__button-change-theme{
    background-color: rgba(255,255,255,0.25);
    color: white;
    align-items: center;
    font-size: 16px;
    border-color: transparent;
    border-radius: 3px;
    min-width: 200px;
    height: 38px;
    cursor: pointer;
    padding: 8px;
    transition: all 0.3s;
    display: flex;
    position: absolute;
    top: 0;
    right: 0;
  }
  .board__button-change-theme img{
    max-width: 50px;
    margin-right: 10px;
  }
  .remove-item {
    float: right;
    color: #a45;
    opacity: 0.5;
    cursor: pointer;
    position: absolute;
    top: 0;
    right: 0;
    display: inline;
    height: 20px;
    width: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .remove-item:hover{
    opacity: 1;
  }
  .board {
    display: flex;
  }
  </style>