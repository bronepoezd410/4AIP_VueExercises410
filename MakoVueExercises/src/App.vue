
<template>
    <ul>
	<li v-for="(elem1, key, index) in obj">
		 {{ key }} - {{ elem1 }} - {{ index+1 }}
    </li>
    </ul>
</template>

<script>
import { normalizeProps } from 'vue';

export default {
    data() {
        return {
            obj: {user1: '100$', user2: '200$', user3: '300$'},
	}
},
    methods: 
    {

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