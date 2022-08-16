<template>
<!-- <div id="content">-->
  <!-- <h1>Ejercicio de preguntas y respuestas haciendo uso de</h1>-->
  <!-- <img alt="" src="https://raw.githubusercontent.com/PokeAPI/media/master/logo/pokeapi_256.png" width="250"> -->
  <!--<HelloWorld msg="Welcome to Your Vue.js App"/>-->
  <!--<ejemploPreguntas/>-->
  <!-- <ejemploFiguras/>-->
<!--</div> -->
<h1 id="title">Ejercicio #3 - Operaciones Básicas de Matrices en VUE</h1>
<ul>
  <li><a href="#syr">Suma y Resta</a></li>
  <li><a href="#ide">Matriz Identidad y Matriz Nula</a></li>
  <li><a href="#pot">Potencia de Matriz</a></li>
  <li><a href="#tra">Matriz Transpuesta</a></li>
  <li><a href="#inv">Inversa</a></li>
</ul>

<div id="matrices">
  <h1 id="syr">Inciso #1</h1>
  <MatrizSumaResta/>
  <h1 id="ide">Inciso #2</h1>
  <matrizIdentidad/>
  <matrizNula/>
  <h1 id="pot">Inciso #3</h1>
  <matrizPot/>
  <matrizPE/>
  <h1 id="tra">Inciso #4</h1>
  <matrizTranspuesta/>
  <h1 id="inv">Inciso #5</h1>
  <matrizGJ/>
</div>
<h1>Grupo #5 - Sistemas Expertos</h1>
<ol>
  <li><strong>Sergio Fabricio Vasquez Castellanos</strong>		- 20142002711</li>
  <li><strong>Angel Santiago Trochez Briones</strong> 	      - 20151021032</li>
  <li><strong>Alexi Daniel Saravia</strong>				          - 20132007687</li>
  <li><strong>Juan De Dios Carranza Motiño</strong> 		      - 20172030613</li>
</ol>
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
span{
    word-spacing: 10px;
  }
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
  color: white;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover {
  background-color: #111;
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
#title{
  color: navy;
  background-color: whitesmoke;
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
