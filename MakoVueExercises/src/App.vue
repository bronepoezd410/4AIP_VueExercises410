
<template>
    <div class="withMargin"> 
        <textarea v-model="input"></textarea>
        <button @click="submit">Submit</button>
    <ul>
      <li v-for="word in words" :key="word">{{ word }}</li>
      <!-- не помню для чего конкретно служит :key -->
    </ul>
    </div>

</template>

<script>
//import { normalizeProps } from 'vue';

export default {
    data() {
        return {
        input: '',
        words: [],
	}
},
    methods: 
    {
        submit() {
      // Split the input into an array of words and update the words data property
      this.words = this.input.split(' ');
    },
    }
}


</script>

<style>

@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');


</style>