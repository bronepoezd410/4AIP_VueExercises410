<template>

	<div>
        <button @click="change">Изменить</button> 
        <button @click="change1">Изменить 2</button> 
        {{ text }}
    </div>

    <div>

        Lorem ipsum dolor sit amet consectetur adipisicing elit. Neque, cupiditate harum facere quia tempore voluptatibus, inventore ex impedit ipsa minima itaque. Quisquam ad tempora <strong>{{ text }}</strong> quia sit aut nobis nemo officiis?

    </div>





</template>

<script>
import { normalizeProps } from 'vue';

export default {
    data() {
	    return {
		text: '',
	    }
    },
    methods: {
	change: function() {
		this.text = 'Я БЕШЕННЫЙ, БЕГИТЕ';

	},
    change1: function(){
        this.text = 'Я НЕНОРМАЛЬНЫЙ'
    }
}
	
	}

</script>

<style>
body{
    background-color: rgb(125, 249, 249);
}
div{
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    font-size: 25px;
    
}

</style>