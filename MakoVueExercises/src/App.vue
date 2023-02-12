<template>
	<p v-if="visible">text</p>
    <br>
    <button @click="hide">hide</button>
    <button @click="show">show</button>
    <button @click="reversal">show/hide</button>

</template>

<script>
import { normalizeProps } from 'vue';

export default {
    data() {
	return {
		visible: false,
	}
    
},
    methods: 
    {
        hide: function() {
		//this.visible = !this.visible;
		this.visible = false;
	    },
        show: function() {
		this.visible = true;
	    },
        reversal: function() {
		this.visible = !this.visible;
        },
    computed: {
    }
    }
}

</script>

<style>



body{
    background-color: rgb(161, 255, 162);
}
div{
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    font-size: 25px;
    
}


</style>