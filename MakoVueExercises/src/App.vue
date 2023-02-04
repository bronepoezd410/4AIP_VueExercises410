<template>

	<div>
	<p>Цена: {{ cost }}</p>
	<p>Количество: {{ amount }}</p>
	<p>Общая стоимость: {{ price }}</p>
    </div>
    
        <button @click="ccost"> Изменить цену </button>






</template>

<script>
import { normalizeProps } from 'vue';

export default {
    data() {
	return {
		cost: 25,
		amount: 200,
	}
    
},
    methods: {
        ccost: function(){
            this.cost = this.cost*2;
        }
},
    computed: {
	    price: function() {
		    return this.cost * this.amount;
	    },
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