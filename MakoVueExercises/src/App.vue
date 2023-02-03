<template>
    <p>{{ arr[0] }}</p>
    <p>{{ arr[1] }}</p>
    <p>{{ arr[2] }}</p>

    <p>{{ arr1[0] + arr1[1] + arr1[2] }}</p>

</template>


<script>
export default {
    name: 'App',
    data() {
	return {
		arr: ['SPHERE', 'CUBE', 'PYRAMID'],
		arr1: [12, 766, 122],
	}
}
}
</script>

<style>

</style>