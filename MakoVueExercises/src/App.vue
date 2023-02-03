<template>

<p>Число {{ num }} в квадрате равняется: {{ num*num }}</p>
<p>Сумма {{num1}} {{num2}} {{num3}} равняется: {{ num1+num2+num3 }}</p>

</template>


<script>
export default {
    name: 'App',
        data() {
	    return {
		num: 5,
        num1: 1,
		num2: 2,
		num3: 3,
	}
    }

	}
</script>

<style>

</style>