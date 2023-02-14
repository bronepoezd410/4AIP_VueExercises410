
<template>
    <div>
	<p v-for="num in 30">
		{{ num }}
	</p>
    </div>

</template>




<script>
import { normalizeProps } from 'vue';

export default {
    data() {
        return {
            
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