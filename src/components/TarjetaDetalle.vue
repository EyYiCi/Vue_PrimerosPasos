<template>
    <div>
       <H1> {{libro.titulo}} </H1>
       <H2>  {{libro.autor}} </H2>

       <H3> {{ mensaje.texto1.toString().toUpperCase() + mensaje.texto2 }}  </H3>

        <div v-html="htmlDatos.dimTexto2"></div>
    </div>
   
    
</template>

<script>
export default {
    name:'TarjetaDetalle',
    data(){
        return {
            libro: {
                autor : "YO merengues",
                titulo: "Lilipot"
            },
            mensaje:{
                texto1:"vueeee",
                texto2:".js"

            },
            htmlDatos:{
                dimTexto:"cadena texto",
                dimTexto2:"<h1>Lorem Input </h1> <i> aqui cursiva </i>"
            }
        }

    }
    
}
</script>

<style scoped>

</style>