<script>
export default{
  'name' : "Login",
   
  data() {},
  methods: {
    onSubmit(){
        this.hendlerLogin()
    }
  },
    props: ['hendlerLogin']
  }
</script>

<template>
<div class="container">
    <div class="form">
        <h1>Авторизация</h1>
        <form v-on:submit.prevent="onSubmit">
            <input placeholder="введите логин" name="login" class="login" type="text"/>
            <input placeholder="введите пароль" name="pasword" class="pass" type="password"/>
            <input type="submit" class="entar"/>
        </form>

    </div>
</div>
</template>
<style scope>
.container{
 background-color:rgba (#fff,0.6);
 height: 100vh;
 width: 100%;
 display: flex;
 align-items: center;
 justify-content: center;
}
.form h1 {
    width: 100%;
    text-align: center;
    color: #fff;
}
.form{
 background-color:rgba(0, 0, 0, 0.6) ;
 width: 600px;
 height: 600px;
 display: flex;
 align-items: center;
 justify-content: center;
}
form{
 background-color:rgba(0, 0, 0, 0.6) 

}
input{
 widows: 80%;
 height: 50px;
 padding: 15px;
}
.enter{

}
.login{

}
.pass{

}
</style>