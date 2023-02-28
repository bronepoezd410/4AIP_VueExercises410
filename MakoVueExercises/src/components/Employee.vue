<template>
	<p>{{ name }} {{ salary }} {{ age }}</p>
</template>



<script>
export default {
    props: ['name', 'salary', 'age'],
    data() {
        return {
        }
    }
}
</script>
