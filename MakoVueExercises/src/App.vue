
<template>
	<p v-if="age < 18">Подросток</p>
	<p v-else-if="age < 26">Молодой человек</p>
	<p v-else>Мужчина</p>
</template>

<script>
import { normalizeProps } from 'vue';

export default {
    data() {
	return {
        age: 25,
	}
},
    methods: 
    {
    computed: 
    {    }


    }
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