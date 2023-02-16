
<template>
    <div class="button_things">
        <button @click="add" class="primary">добавить </button>   
        <br>
        <button @click="removeb" class="primary">убрать первый</button> 
        <br>    
        <button @click="removef" class="primary">убрать последний</button> 
        <br>    
        <button @click="removel" class="primary">убрать предпоследний</button> 
        <br>    
        <button @click="sort1" class="primary">отсортировать</button> 
        <br>    
        <button @click="reverse1" class="primary">перевернуть</button> 
    <br>    
    </div>
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


@import url('./style.css');
@import url(./baton_styles.css);
</style>