
<template>
    <ul>
	<li v-for="(elem, key) in arr">
		 {{ key }} {{ elem }}
    </li>
    </ul>
</template>

<script>
import { normalizeProps } from 'vue';

export default {
    data() {
        return {
        arr: ['x', 'y', 'z'],
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