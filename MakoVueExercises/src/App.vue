
<template>
    <div class="withMargin"> 
    <p>Какие языки вы знаете?</p>
    <input type="checkbox" v-model="arr" value="russian"> Русский
	<input type="checkbox" v-model="arr" value="english"> Английский
	<input type="checkbox" v-model="arr" value="french"> Французский

    <ul>
        <li v-for="items in arr"> {{ items }} </li>

    </ul>

    </div>


</template>

<script>
//import { normalizeProps } from 'vue';

export default {
    data() {
        return {
            arr: [],
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