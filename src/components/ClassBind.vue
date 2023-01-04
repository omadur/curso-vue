<template>
    <!--bindear datos (etiqueta clase) -->
    <p v-bind:class="{'danger' : hasError}">El mensaje se ha enviado satisfactoriamente.</p>

    <!--bindear datos (etiqueta style) -->
    <p v-bind:style="{backgroundColor:'#ccc', color: color}">El mensaje se ha enviado satisfactoriamente.</p>

    <button v-on:click="handleClick">Cambiar color</button>
</template>

<script>
// Utilizando el setup solo se colocaria la linea let hasError = true;
    import { defineComponent } from 'vue';
    import { ref } from 'vue';
    export default defineComponent({
        name:'ClassBind',
        setup(){
            let hasError = true;
            let color = ref('#ff5');

            const handleClick = () => color.value = 'red';

            return {hasError, color, handleClick}
        }
    })
</script>

<style scoped>
    .danger{
        color: red;
    }

</style>