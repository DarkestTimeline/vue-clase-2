<template>
  <!--<img alt="Vue logo" src="./assets/sis_logo.png" width="300">-->
  <!--<HelloWorld msg="Welcome to Your Vue.js App"/>-->
  <!--<ejemploPreguntas/>-->
  <ejemploFiguras/>
</template>

<script>
//import EjemploPreguntas from './components/EjemploPreguntas.vue'
import EjemploFiguras from './components/EjemploFiguras.vue'
// import HelloWorld from './components/HelloWorld.vue'



export default {
  name: 'App',
  components: {
    // HelloWorld
    //EjemploPreguntas,
    EjemploFiguras
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
