
<template>
    <ul>
	<div v-for="elem in items">
        <li>
        {{ elem }}
        </li>
        <li class="divider">divider</li>
    </div>
    </ul>
</template>

<script>
import { normalizeProps } from 'vue';

export default {
    data() {
        return {
		items: [1, 2, 3],
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