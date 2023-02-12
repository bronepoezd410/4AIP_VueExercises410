
<template>
    <p v-if="isAdmin">+++</p>
    <p v-else>---</p>
    
	<button @click="allo"> {{ isAdmin ? 'hide' : 'show' }} </button>
</template>

<script>
import { normalizeProps } from 'vue';

export default {
    data() {
	return {
		isAdmin: true,
	}
},
    methods: 
    {
        allo: function() {
        this.isAdmin = !this.isAdmin;
        
    },
    computed: 
    {    }


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