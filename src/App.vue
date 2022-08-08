<template>
<!-- <div id="content">-->
  <!-- <h1>Ejercicio de preguntas y respuestas haciendo uso de</h1>-->
  <!-- <img alt="" src="https://raw.githubusercontent.com/PokeAPI/media/master/logo/pokeapi_256.png" width="250"> -->
  <!--<HelloWorld msg="Welcome to Your Vue.js App"/>-->
  <!--<ejemploPreguntas/>-->
  <!-- <ejemploFiguras/>-->
<!--</div> -->
<div id="matrices">
  <h1>Inciso #1</h1>
  <MatrizSumaResta/>
  <h1>Inciso #2</h1>
  <matrizIdentidad/>
  <matrizNula/>
  <h1>Inciso #3</h1>
  <matrizPot/>
  <matrizPE/>
  <h1>Inciso #4</h1>
  <matrizTranspuesta/>
  <h1>Inciso #5</h1>
<matrizGJ/>
</div>
<h2>Grupo #5 - Sistemas Expertos</h2>
<img alt="" src="./assets/sis_logo.png" id="sis_logo">
  
</template>

<script>
// import EjemploPreguntas from './components/EjemploPreguntas.vue'
// import EjemploFiguras from './components/EjemploFiguras.vue'
// import HelloWorld from './components/HelloWorld.vue'
import MatrizGJ from './components/MatrizGJ.vue'
import MatrizPE from './components/MatrizPE.vue'
import MatrizPot from './components/MatrizPot.vue'
import MatrizTranspuesta from './components/MatrizTranspuesta.vue'
import MatrizIdentidad from './components/MatrizIdentidad.vue'
import MatrizNula from './components/MatrizNula.vue'
import MatrizSumaResta from './components/MatrizSumaResta.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
    // EjemploPreguntas,
    // EjemploFiguras
    MatrizTranspuesta,
    MatrizGJ,
    MatrizPot,
    MatrizPE,
    MatrizIdentidad,
    MatrizNula,
    MatrizSumaResta
}
}
</script>

<style>
*,
*:before,
*:after {
  box-sizing: border-box;
}
img{
  width: 20%;
}
h1 {
  border-radius: 15px;
  background-color: rebeccapurple;
  color: whitesmoke;
}
input[type=radio] {
  border: 0px;
  width: 10%;
  height: 2em;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#content{
  background-color: rgb(254, 202, 27, 0.7);
  margin: 0px 50px;
  padding: 5px 20px;
  border-radius: 5%;
  border: 5px solid #264375;
}
#matrices{
  margin: 0px 150px;
  padding: 5px 20px;
  border-radius: 5%;
}
#sis_logo{
  width: 150px;
}
#res{
  color: whitesmoke;
  background-color: #406bb5;
  border-radius: 5px;
}

</style>
