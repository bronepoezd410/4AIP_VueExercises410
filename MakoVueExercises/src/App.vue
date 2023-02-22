
<template>
    <div class="withMargin"> 
        <input type="checkbox" v-model="checked">
	    <p v-if="checked">aloha</p>
    </div>

</template>

<script>
//import { normalizeProps } from 'vue';

export default {
    data() {
        return {
		checked: true,
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