<template>
  <div id="app">
    <!-- <TarjetaBucles></TarjetaBucles> 
    <TarjetaDetalle></TarjetaDetalle> 
    <TarjetaBoton v-for="x in 8" v-bind:key="x"></TarjetaBoton>
    -->
    <TarjetaBoton></TarjetaBoton>
  </div>
</template>

<script>
import {defineComponent} from 'vue';
//import TarjetaBucles from './components/TarjetaBucles.vue';
//import TarjetaDetalle from './components/TarjetaDetalle.vue';
import TarjetaBoton from './components/TarjetaBoton.vue';

export default defineComponent ({
  name: 'app',
  components: {
    //TarjetaDetalle,
    //TarjetaBucles,
    TarjetaBoton
  }
});
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
