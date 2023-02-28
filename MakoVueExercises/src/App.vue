
<template>
    <div class="withMargin"> 
        <input v-model="message" @keyup.enter="submit"/>
        <p> {{ actualmessage  }}</p>

        <a href="#" @click.alt="show" > ссылка </a>
        <p>{{ text }}</p>


        <a href="#" @click.left="displayText('left')" @click.right="displayText('right')" @click.middle="displayText('middle')">Click me!</a>
        <p>{{ text1 }}</p>


    </div>


</template>

<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
        message: '',
        actualmessage: '',
        text: '',
        text1: ''

    }
  },
    methods: 
    {
        submit: function(){
            this.actualmessage = this.message

        },
        show: function(){
            this.text = 'ALT key is pressed!'
        },
        displayText(button) {
        if (button === 'left') {
            this.text1 = 'left'} 
            else if (button === 'right') {
            this.text1 = 'right'} 
            else if (button === 'middle') {
            this.text1 = 'middle'
        }
    }

    }
}


</script>

<style>

@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');


</style>