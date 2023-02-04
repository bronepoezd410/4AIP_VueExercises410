
<template>
	<button @click="show(2)">Получить квадрат числа два</button>
	<button @click="show(3)">Получить квадрат числа три</button>
</template>

<script>
import { normalizeProps } from 'vue';

export default {
    data() {
	    return {

	    }
    },
	methods: {
	show: function(int) {
        alert(int * int);
	},

    }
	
	}

</script>

<style>

</style>