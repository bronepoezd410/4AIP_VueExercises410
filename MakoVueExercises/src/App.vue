
<template>
    <button @click="delogin"> {{ isAuth ? 'hide' : 'show' }}</button>
	<div v-if="isAuth">
		<p>+++</p>
		<p>+++</p>
		<p>+++</p>
	</div>
</template>

<script>
import { normalizeProps } from 'vue';

export default {
    data() {
	return {
        isAuth: true,
	}
},
    methods: 
    {
        delogin: function(){
            this.isAuth = !this.isAuth
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