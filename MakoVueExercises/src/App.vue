
<template>
    <div class="withMargin"> 
        <p>В каком городе вы живете?</p>
        <select v-model="selected">
		<option>Саратов</option>
		<option>Брянск</option>
		<option>Калуга</option>
	    </select>
	
	<p>{{ selected }}</p>

    <p v-if="choice == 'Английский'"></p>



    </div>


</template>

<script>
//import { normalizeProps } from 'vue';

export default {
    data() {
        return {
            selected: 'value1', // значение по умолчанию
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