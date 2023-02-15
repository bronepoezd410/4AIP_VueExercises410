
<template>


<div class="header" style="background-color: #334d5c; color: #fff; padding: 20px;">
    <h1 style="color: #fff; font-size: 32px;">David's Laboratory</h1>
    <nav style="background-color: #1e1e1e; color: #fff; padding: 10px;">
      <a href="#">Home</a>
      <a href="#">About</a>
      <a href="#">Services</a>
      <a href="#">Contact</a>
    </nav>
  </div>


    <button @click="add" class="button button-primary">добавить </button>   
    <br>
    <button @click="removeb" class="button button-secondary">убрать первый</button> 
    <br>    
    <button @click="removef" class="button button-secondary">убрать последний</button> 
    <br>    
    <button @click="removel" class="button button-secondary">убрать предпоследний</button> 
    <br>    
    <button @click="sort1" class="button button-secondary">отсортировать</button> 
    <br>    
    <button @click="reverse1" class="button button-secondary">перевернуть</button> 
    <br>    


    <ul>
        <li v-for="elem in arr">
            <a> {{ elem }}</a>
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

@import url(./style.css);



</style>