
<template>
    <button @click="add">добавить </button>   
    <br>
    <button @click="removeb">убрать первый</button> 
    <br>    
    <button @click="removef">убрать последний</button> 
    <br>    
    <button @click="removel">убрать предпоследний</button> 
    <br>    
    <button @click="sort1">отсортировать</button> 
    <br>    
    <button @click="reverse1">перевернуть</button> 
    <br>    

    <ul>
        <li v-for="elem in arr">
            <p> {{ elem }}</p>
        </li>
    </ul>
</template>




<script>
import { normalizeProps } from 'vue';

export default {
    data() {
        return {
		arr: ['1', '2', '3'],
	}
},
    methods: 
    {
        add: function() {
		this.arr.push(this.arr.length); // добавить элемент
        },
        removeb: function(){
        this.arr.shift(0) // убрать первый
        },
        removef: function(){
        this.arr.splice(this.arr.length-1) //убрать последний
        },
        removel: function(){
        this.arr.splice(this.arr.length-2, 1) //убрать предпоследний
        },
        sort1: function(){
        this.arr.sort() //отсортировать
        },
        reverse1: function(){
        this.arr.reverse() //отсортировать
        },

    computed: 
    {    
    }


    }
}

</script>

<style>



body{
    background-color: rgb(161, 255, 162);
}
div{
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    font-size: 40px;
    
}


table, th, td {
  border: 3px solid black;
  border-collapse: collapse;
}


button {
    font-size: 30px;
    border: 4px solid orange;
    margin: 5px;
	}

</style>