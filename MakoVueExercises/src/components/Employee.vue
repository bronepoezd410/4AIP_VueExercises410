<script>
export default {
    emits: ['show', 'show1'],
    data() {
        return {
        }
    },
    methods: {
        handleName() {
            this.$emit('show', 'Давид Авагян');
        },
        handleSalary(){
            this.$emit('show1', '12');
        }
    }
}
</script>


<template>
	<button class="button" @click="handleName">Name</button>
	<button class="button" @click="handleSalary">Salary</button>
</template>


<!-- props: {
	title: String,
	likes: Number,
	isPublished: Boolean,
	commentIds: Array,
	author: Object,
	callback: Function,
	contactsPromise: Promise // или любой другой конструктор
} -->