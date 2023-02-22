
<template>
    <div class="withMargin"> 



	<!-- <button @click="disabl">btn</button> -->
    <input type="checkbox" v-model="isDisabled">

    <input v-bind:disabled="isDisabled" type="text">
    </div>


</template>

<script>
//import { normalizeProps } from 'vue';

export default {
  data() {
    return {
		isDisabled: false,
    }
  },
    methods: 
    {
        disabl: function (){
            this.isDisabled = !this.isDisabled
        }
    }
}


</script>

<style>

@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');


</style>