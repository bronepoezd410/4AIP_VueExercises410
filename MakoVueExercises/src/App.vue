<template>


	<button @click="show">Показать</button>

</template>


<script>
export default {
    data() {
	    return {
		    number1: 100,
		    number2: 211,
	    }
    },
	methods: {
		show: function() {
            alert(this.number1 + this.number2);

        }
	}
}

</script>

<style>

</style>