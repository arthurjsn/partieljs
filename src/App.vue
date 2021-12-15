<template>
  <titre msg="Tringle Rail"/>
  <img alt="Image tringle" src="./assets/logo.jpg">

  <div v-if="step='step0'">
    <Dimension />
    <button v-on:click="step='step1'">VALIDER</button>
  </div>

  <div v-if="step='step1'">
    <Type />
    <button v-on:click="step='step2'">VALIDER</button>
  </div>

  <div v-if="step='step2'">
    <Couleur />
    <button v-on:click="step='step3'">VALIDER</button>
  </div>

  <div v-if="step='step3'">
    <Nombrerideaux />
    <button v-on:click="step='step4'">VALIDER</button>
  </div>

  <div v-if="step='step4'">
    <Nombrerideaux />
    <button>VALIDER</button>
  </div>

</template>

<script>
import Dimension from './components/Dimension.vue'
import Titre from './components/Titre.vue'
import Couleur from './components/Couleur.vue'
import Type from './components/Type.vue'
import Nombrerideaux from './components/Nombrerideaux.vue'
export default {
  
  data() 
  {
    return {
      step: "step0"
    };
  },

  name: 'App',
  components: {
    Titre,
    Dimension,
    Couleur,
    Type,
    Nombrerideaux,  }
}
</script>

<style>

img {
  width: 30%;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
