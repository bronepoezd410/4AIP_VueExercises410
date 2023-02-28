<template>

    <div class="withMargin">
        <p>промежуточная ветвь! </p>
    </div>


    <User/>


</template>

<script>
import User from './components/User.vue'
	

export default {
    data() {
	return {
        components: {
			User
		}
	}
},
    methods: 
    {
    }

}


</script>

<style>

@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');


</style>