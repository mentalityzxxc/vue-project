<script>
    export default {
        'name':"board",
        data(){
            return{
            hello:"privet",
            wallpapers:[
                "https://i.pinimg.com/originals/b3/cf/82/b3cf8221bf35baf3d4faa68473811fc9.jpg",
                "https://www.passion.ru/thumb/1500x0/filters:quality(75):no_upscale()/imgs/2022/03/24/16/5323877/30c1e09df2ea3734f0635eb503b486865d338c36.jpg",
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
              },
              {
                id: '2',
                title: 'нанять строителей',
              },
              {
                id: '3',
                title: 'покрасить стены',
              }
            ],
            inprogress: [
              {
               id: '4',
                title: 'закупить инструменты',
              },
              {
                id: '5',
                title: 'заказать стеклопакет',
              },
              {
                id: '6',
                title: 'заказать мебель',
              }
            ],
             done: [
              {
                id: '7',
                title: 'выплатить ЗП',
              },
              {
                id: '8',
                title: 'оформить документы',
              },
              {
                id: '9',
                title: 'сделать фото отчет',
              }
            ],
            };
        },
        props: ['test'],
        methods: {
               handlerDragend(event, type){
            let Element = document.elementFromPoint(event.x, event.y)
           // console.log(element)
            if(Element.getAttribute('class') == 'drop-zone') {
              const id = event.target.getAttribute('id')
              let arrayFrom = this[type];
              let element = arrayFrom.find(el => el.id == id)            
              let filterNewArray = arrayFrom.filter(el => el.id !== id)
              this[type] = filterNewArray
              let arrayTo = Element.getAttribute('name')
              this[arrayTo].unshift(element);
              //console.log(type)
            }
          },  
          changeBackground(number){
            this.currentWallpaper = number
            this.activeMenu = false;
          },
          openCloseMenu(){
            //alert('функция отроботона')
            //this.activeMenu = true;
            if (this.activeMenu) {
              this.activeMenu = false;
            } else {
              this.activeMenu = true;
            }
          }
        }
    }
</script>

<template>
<div>
  <div class='board' :style="{'background-Image':`url('${wallpapers[currentWallpaper]}')`}">
      <button class='board__button-change-theme' @click='openCloseMenu'>
        <img :src='wallpapers[currentWallpaper]' />Сменить фон
      </button>
    <div :class="[activeMenu ? 'board__theme-wrapper board__theme-wrapper--active' : 'board__theme-wrapper']">
        <div id="wallpapers">
          <div v-for="(item, i) in wallpapers"
            class='wallpapers__item'
            :key="index"
            :style="{'background-Image':`url('${item}')`}"
            @click='changeBackground(i)'>
          </div>
        </div>
      <div class='close-wallpapers' @click='openCloseMenu'>
      {{'<'}}
    </div>
  </div>
      <section class='board-content'>
          <h2>
           Надо сделать
          </h2>
          <input placeholder='Новый товар'
          class='new-todo todo-item'
          >
          <div class='drop-zone'
          name='list'>
          <img src='public/assets/cursor.png'>
          </div>
          <ul class='todo-list board__column'>
          <li class='todo-item shoping__item'
           v-for="(item, index) in list"
          :key="item.id"
          draggable="true"
          @dragend="handlerDragend($event, 'list')"
          :id='item.id'>
           {{ item.title }}
          </li>
          </ul>
      </section>
      <section class='board-content'>
          <h2>
           В процессе
          </h2>
          <input placeholder='Новый товар'
          class='new-todo todo-item'
          >
          <div class='drop-zone'
          name='inprogress'>
          <img src='public/assets/cursor.png'>
          </div>
          <ul class='todo-list board__column'>
          <li class='todo-item shoping__item'
           v-for="(item, index) in inprogress"
          :key="item.id"
          draggable="true"
          @dragend="handlerDragend($event, 'inprogress')"
          :id='item.id'>
           {{ item.title }}
          </li>
          </ul>
      </section>
            <section class='board-content'>
          <h2>
           Выполнено
          </h2>
          <input placeholder='Новый товар'
          class='new-todo todo-item'
          >
          <div class='drop-zone'
          name='done'>
          <img src='public/assets/cursor.png'>
          </div>
          <ul class='todo-list board__column'>
          <li class='todo-item shoping__item'
           v-for="(item, index) in done"
          :key="item.id"
          draggable="true"
          @dragend="handlerDragend($event, 'done')"
          :id='item.id'>
           {{ item.title }}
          </li>
          </ul>
      </section>
    </div>
</div>
</template>

<style scoped>
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
      display: flex;
      justify-content: center;
      position: absolute;
      width: 100%;
      left: 0;
      top: 0;
      height: 100%;
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
  body {
    font-family: "Source Sans Pro", "Arial", sans-serif;
  }
  * {
    box-sizing: border-box;
  }
  .board section{
    width: 30%;
    margin: 5px;
  }
  .todo-list {
    list-style-type: none;
    padding: 10px;
  }
  .done {
    text-decoration: line-through;
    color: #888;
  }
  .new-todo {
    width: 100%;
  }
  .trash-drop {
    border: 2px dashed #ccc !important;
    text-align: center;
    color: #e33;
  }
  .trash-drop:-moz-drag-over {
    border: 2px solid red;
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
  </style>