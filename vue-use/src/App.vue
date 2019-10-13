<template>
  <div id="app">
    <img src="./assets/logo.png">
    <ELButton type="primary"></ELButton>
    <router-view/>
  </div>
</template>

<script>
import Helloworld from './components/HelloWorld'
import AVue from '@/AVue.js'
export default {
  name: 'App',
  components:{
    Helloworld
  },
  mounted(){
    this.$message('请确认支付')
    // const av = new AVue({
         
    // })
    this.$alert();
  },
  created(){
    console.log('1')
    class SingleDog{
        show(){
          console.log('我是一个单例对象')
        }
        static getInstance(){
          if(!SingleDog.instance){
            SingleDog.instance = new SingleDog();
          }
          return SingleDog.instance
        }
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
