<script>
    export default {
        'name':"board",
        data(){
            return{
            hello:"privet",
            wallpapers:[
                   'https://i.pinimg.com/originals/b3/cf/82/b3cf8221bf35baf3d4faa68473811fc9.jpg',
                    'https://www.passion.ru/thumb/1500x0/filters:quality(75):no_upscale()/imgs/2022/03/24/16/5323877/30c1e09df2ea3734f0635eb503b486865d338c36.jpg'
            ]
            };
        },
        props: ['test']
    }
</script>

<template>
  <div>
    {{ hello }}
    {{ test }}
    <li v-for="item in wallpapers">
    {{ item }}
    <img :src="item">
    </li>
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
    left: 0;
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