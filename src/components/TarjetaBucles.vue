<template>
    <div>
       <ul>
           <li v-for="color in colores" v-bind:key="color"> {{color}} </li>

       </ul>

       <div v-for="coloro in colorobj" v-bind:key="coloro">
            ESPAÑOL : {{coloro.nombre}} <br>
            ENGLISH : {{coloro.nombreIngles}}

            <p>------------------------------------------</p>
        </div>
    </div>
    
  
</template>

<script>
import {defineComponent} from "vue";

export default defineComponent ({
    name: "TarjetaBucles",
    data(){
        return {
            colores: ["rojo", "verde","amarillo","azul"],
            colorobj:[
                { nombre:"rojo", nombreIngles:"red" },
                { nombre:"azul", nombreIngles:"blue" },
                { nombre:"amarillo", nombreIngles:"yellow" },
                { nombre:"rosa", nombreIngles:"pink" },
            ]
        }
    }
});
</script>
<style scoped>

</style>