<template>
    <div>
        <hr>
        <div v-if="mostrarBoton == 'agc'">
          Usuario autenticado  <button> Boton secreto </button>
        </div>
        <div v-else-if="agc">
            Error
        </div>
    </div>
    
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
    name:"TarjetaBoton",
    data(){
        return {
            mostrarBoton: "agc"
        }
    }
});
</script>

<style scoped>

</style>