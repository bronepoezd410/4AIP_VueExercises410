<template>

    <p>
    <a href="{{href}}"><img :src="attr" 
    width="200" height="200" alt="david">
    </a>
    Давид джентельмен как ни крути на вид...
    </p>

    <a href={{href}}>{{text}}</a>


</template>


<script>
export default {
    name: 'App',

    data() {
	return {
		text: 'zamayproject',
		href: './zamayproject.html',
        attr: "./assets/david.jpg"

	}
}
}
</script>

<style>

</style>