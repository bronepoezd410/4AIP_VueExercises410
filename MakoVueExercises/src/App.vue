
<template>
	<div>
    <ul>
        <li v-for = "jopa in hrefs">
            <a href= {{jopa.href}}> {{jopa.text}} </a>
        </li>
    </ul>
    </div>

    <div>
        <table>
            <tr v-for="things in products">
                <td> {{ things.name }} </td>
                <td> {{ things.price }} </td>
                <td> {{ things.quantity }} </td>
            </tr>
        </table>
    </div>

</template>




<script>
import { normalizeProps } from 'vue';

export default {
    data() {
        return {
            hrefs: [
			{href: '1.html', text: 'text1'},
			{href: '2.html', text: 'text2'},
			{href: '3.html', text: 'text3'},
		],
        products: [
			{
				name: 'product1',
				price: 100,
				quantity: 5
			},
			{
				name: 'product2',
				price: 200,
				quantity: 4
			},
			{
				name: 'product3',
				price: 300,
				quantity: 3
			},
		],

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