
<template>
	<p v-if="day === 1">Понедельник</p>
	<p v-if="day === 2">Вторник</p>
	<p v-if="day === 3">Среда</p>
	<p v-if="day === 4">Четверг</p>
	<p v-if="day === 5">Пятница</p>
	<p v-if="day === 6">Суббота</p>
	<p v-if="day === 7">Воскресенье</p>
</template>

<script>
import { normalizeProps } from 'vue';

export default {
    data() {
	return {
		day: 4,
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