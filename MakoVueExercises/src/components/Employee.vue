
<template>
<ul>

	<li v-for="names in name">{{ names }}</li>
</ul>
</template>



<script>
export default {
	props: ['name'],	
    data() {
        return {
        }
    }
}
</script>
