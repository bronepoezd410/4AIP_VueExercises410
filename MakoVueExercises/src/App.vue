
<template>
    <div>
    <template v-for="num in items">
	    <p v-if = "num> 0">
		    {{ num }}
	    </p>
    </template>

    </div>

</template>




<script>
import { normalizeProps } from 'vue';

export default {
    data() {
        return {
		items: [1, -2, 3, -4, 5],
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


table, th, td {
  border: 3px solid black;
  border-collapse: collapse;
}

</style>