<template>

<!-- обработчик click будет вызван максимум 1 раз -->
<!-- <a @click.once="doThis"></a> -->
    <button><a @click.once="plusinteger">{{ integer }}</a></button>

    <button><a @click.prevent href="http://github.com/bronepoezd410/">GitHub</a></button>



</template>

<script>
import { normalizeProps } from 'vue';

export default {
    data() {
	return {
        integer: 13
	}
    
},
    methods: {
        plusinteger: function(){
            this.integer = this.integer * 2;

        }
    },
    computed: {}
}

</script>

<style>
body{
    background-color: rgb(64, 5, 65);
}
div{
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    font-size: 25px;
    
}


</style>