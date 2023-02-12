<template>


	<button @click="toggle">toggle</button>
	<p v-if="visible">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Vel assumenda minus eveniet quam laudantium veritatis dignissimos atque, quasi tenetur quae.</p>
<br>
    <button @click="toggle1">toggle</button>
    <p v-if="visible1">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Vel assumenda minus eveniet quam laudantium veritatis dignissimos atque, quasi tenetur quae.</p>
<br>
    <button @click="toggle2">toggle</button>
    <p v-if="visible2">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Vel assumenda minus eveniet quam laudantium veritatis dignissimos atque, quasi tenetur quae.</p>


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