
<template>
<ul>
	<li v-for="elem in items">{{ elem**2 }}</li>
</ul>

</template>

<script>
import { normalizeProps } from 'vue';

export default {
    data() {
        return {
		items: [1, 2, 3, 4, 5],
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