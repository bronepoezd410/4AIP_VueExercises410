<template>
	<p>{{ name }} {{ salary }} {{ age }}</p>
</template>


<script>
export default {
	props: {
		name: String,
		salary: String,
		age: Number,
	},
    data() {
        return {
        }
    }
}
</script>

<!-- props: {
	title: String,
	likes: Number,
	isPublished: Boolean,
	commentIds: Array,
	author: Object,
	callback: Function,
	contactsPromise: Promise // или любой другой конструктор
} -->