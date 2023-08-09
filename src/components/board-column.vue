<script>
    export default {
        name: "BoardColumn",
        data() {
            return {
                renderCount: 0,
                checkedTask: 0
            }
        },
        props: [
            'title', 
            'items', 
            'name', 
            'handlerDragend', 
            'taskModel', 
            'addTask', 
            'delTask', 
            'editTask'
        ],
        methods: {
            update(){
                this.renderCount = this.renderCount + 1;
                //Вызываем функцию, для подсчета выделенных задач и обновляем состояние
                //Которое отвечает за вывод количества выделенных задач
                this.checkedTask = this.getColumnCheckedCount();
            },
            //Метод, который возвращает количество задач в колонке
            getColumnCount(){
                //Получаем количество объектов в колонке 
                let countInColumn = this.items.length;
                //Возвращаем длинну
                return countInColumn
            },
            //Метод, который получает выбранные элементы
            getColumnCheckedCount(){
                //Заведем переменную в которую запишем все выделенные задачи
                let checkedTasks = this.items.filter(function(item){
                    //Проверяем, что задача выбрана и возвращаем в отфильтрованный массив
                    if (item.checked) {
                        // Возвращаем в отфильтрованный массив элеменит, если он выбран
                        // Галочка в значении true
                        return item
                    }
                })
                //Возвращаем количество выранных задач
                return checkedTasks.length;
            }
        }
    }
</script>
<template>
    <section class='board-content'>
          <h2>
            {{title}}
          </h2>
          <input 
            placeholder='Новый товар'
            type='text'
            class='new-todo todo-item'
            v-model="taskModel"
            v-on:keyup.enter="addTask(taskModel, name)"
          >
          <div 
            class='drop-zone'
            :name='name'
          >
            <img src='public/assets/cursor.png'>
          </div>
          <p class='check-task'>Количество задач: {{getColumnCount()}}</p>
          <p class='check-task'>Выделено задач: {{checkedTask}}</p>
          <p class='check-task'>
            Пользователь выбрал задачу из колонки {{renderCount}} количество раз
          </p>
          <ul class='todo-list board__column'>
              <li 
                class='todo-item shoping__item'
                v-for="(item, index) in items"
                :key="item.id"
                draggable="true"
                @dragend="handlerDragend($event, name)"
                :id="item.id"
              >
                {{ item.title }}
                <div>
                    <button @click="editTask(item.id, name)">Редактировать</button>
                    <button @click="delTask(item.id, name)">Удалить</button>
                    <p>
                        <label>
                            Выделить
                            <input type='checkbox' @click='update' :checked='item.checked' v-model='item.checked'/>
                        </label>
                    </p>
                </div>
              </li>
          </ul>
      </section>
</template>
<style scoped>
.check-task{
    color: white;
    font-size: 20px;
}
body{
    font-family: "Source Sans Pro", "Arial", sans-serif;
}
*{
    box-sizing: border-box;
}
.drop-zone{ 
    background: white;
    height: 150px;
    display: flex;
    align-items: center;
    justify-content: center;
  }
.drop-zone img{
    max-width: 50px;
    margin: 10px;
}
.board__column{
    background-color: #ededed;
    text-align: center;
    min-width: 100%;
    min-height: 80vh;
  }
.board__column--in-stock{
    width: 30%;
    min-width: 300px;
}
.board section{
    width: 30%;
    margin: 5px;
}
.new-todo {
    width: 100%;
}
.todo-list {
    list-style-type: none;
    padding: 10px;
}
.todo-item {
    position: relative;
    border: 1px solid #ccc;
    border-radius: 2px;
    padding: 14px 8px;
    margin-bottom: 3px;
    background-color: #fff;
    box-shadow: 1px 2px 2px #ccc;
    font-size: 22px;
    color: black;
}
.shoping__item a{
    display: flex;
    align-items: center;
    color: black;
  }
.shoping__item:hover{
    box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;
}
.shoping__title{
    font-size: 24px;
}
.done {
    text-decoration: line-through;
    color: #888;
}
.trash-drop {
    border: 2px dashed #ccc !important;
    text-align: center;
    color: #e33;
}
.trash-drop:-moz-drag-over {
    border: 2px solid red;
}
.shoping__img{
    max-width: 50px;
    margin-right: 20px;
}
ul{
    list-style: none;
}
.shoping__item{
    background-color: white;
    color: black;
    margin: 15px 0;
    padding: 10px;
    border-radius: 15px;
}
</style>
