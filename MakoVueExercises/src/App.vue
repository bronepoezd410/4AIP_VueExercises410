<template>

<!-- обработчик click будет вызван максимум 1 раз -->
<!-- <a @click.once="doThis"></a> -->
<!-- <a v-if="visible" href="http://github.com/bronepoezd410/">GitHub</a> -->
    <p v-if = "!hidden">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Deserunt, sit. Veritatis quidem illo, aspernatur distinctio nisi quaerat ab dolor eius incidunt recusandae consequuntur, officia hic, dolores sunt nam similique iure deserunt quis rerum ratione. Culpa maiores dolorum tenetur natus earum.</p>


</template>

<script>
import { normalizeProps } from 'vue';

export default {
    data() {
	return {
        hidden: false
	}
    
},
    methods: {},
    computed: {}
}

</script>

<style>
body{
    background-color: rgb(161, 255, 162);
}
div{
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    font-size: 25px;
    
}


</style>