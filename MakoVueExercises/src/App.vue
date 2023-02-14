
<template>
    <div>
        <ul>
            <li v-for="things in products" :key="things.id">
                {{ things.name }}



            </li>


        </ul>

    </div>

</template>




<script>
import { normalizeProps } from 'vue';

export default {
    data() {
        return {
            products: [
			{
				id: 1,
				name: 'product1',
			},
			{
				id: 2,
				name: 'product2',
			},
			{
				id: 3,
				name: 'product3',
			},
		]
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