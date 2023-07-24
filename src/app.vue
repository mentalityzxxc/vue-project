<script>
import Board from './components/bord.vue'
import Login from './components/login.vue'

export default{
  'name' : "App",
    data(){
        return {
          isAuth: false,
          users: [{
              login:'admin',
              password:'admin'
          }
          ]
        }
    },
  components:{
    Board,
    Login
  },
  methods: {
    login(){
      console.log('авторизация')
    }
  },
}
</script>

<template>
  <Board test='test props' v-if="isAuth"/>
  <login :hendlerLogin="login" v-else/>
</template>

<style scoped>
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
