<template>
  <div id="app">
    <!--<img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>-->
    <p>{{count}}</p>
    <button @click="add">点我+</button>
    <button @click="sub">点我-</button>
  </div>
</template>

<script>
//import { METHODS } from 'http';
//import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  /*components: {
    HelloWorld
  }*/
  data:function(){
    return{
      count:0
    };
  },
  methods:{
    add:function(){
      this.count++;
    },
    sub:function(){
      this.count--;
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
