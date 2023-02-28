
<template>
    <div class="withMargin"> 
	<input v-model="newItem">
	<button @click="addItem" >add to ending</button>
	<button @click="addItemToBegin" >add to beginning</button>

    <ul>
		<li v-for="(item, index) in items" :key="index">
			{{ item }}
		</li>
	</ul>



    </div>


</template>

<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
        newItem: '',
		items: ['a', 'b', 'c', 'd', 'e'],

    }
  },
    methods: 
    {
	addItem: function() {
		this.items.push(this.newItem);
	},
	addItemToBegin: function() {
		this.items.unshift(this.newItem);
	}
    }

    }


</script>

<style>

@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');


</style>