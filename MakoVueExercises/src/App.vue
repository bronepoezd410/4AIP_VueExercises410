<template>

    <p>{{ object.a + object.b + object.c }}</p>

</template>


<script>
export default {
    name: 'App',
    data() {
	return {
		object: {a: 10, b: 20, c: 30},
	}
}
}
</script>

<style>

</style>