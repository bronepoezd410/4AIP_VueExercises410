
<template>
	<button @click="toggle"> {{ visible ? 'hide' : 'show' }} </button>
    <p v-if="visible">text</p>
    <br>

	<button @click="toggle1"> {{ visible1 ? 'hide' : 'show' }} </button>
    <p v-if="visible1">text</p>
    <br>

	<button @click="toggle2"> {{ visible2 ? 'hide' : 'show' }} </button>
    <p v-if="visible2">text</p>
</template>

<script>
import { normalizeProps } from 'vue';

export default {
    data() {
	return {
		visible: false,
		visible1: false,
		visible2: false,
	}
    
},
    methods: 
    {
        toggle: function() {
	    this.visible = !this.visible;
    },
        toggle1: function() {
	    this.visible1 = !this.visible1;
    },
        toggle2: function() {
	    this.visible2 = !this.visible2;
    },
    computed: 
    {

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