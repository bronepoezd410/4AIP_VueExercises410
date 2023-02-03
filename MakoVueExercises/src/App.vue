<template>

<button @click="showdate">Показать текущую дату НАЖАТЬ</button>
<button @mouseenter="showdate">Показать текущую дату НАВЕСТИ</button>

</template>


<script>
export default {
	data() {
		
	},
	methods: {
		showdate: function() {
            // Simply create a new Date object and pass it to alert()
            alert(new Date());

        }
	}
}
</script>

<style>

</style>