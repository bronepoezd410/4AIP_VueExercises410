
<template>
    <div class="withMargin"> 
        <input type="number" v-model="num" class="my-input">
        <button v-on:click="calc">Квадратировать </button>
        <p>Квадрат введенного числа: {{ res }}</p>
    </div>

    <div class="withMargin">
        <input type="number" v-model="number1" class="my-input">
        <input type="number" v-model="number2" class="my-input">
        <button v-on:click="summ">Сложить </button>
        <p>Сумма введенных чисел: {{ resnumber }}</p>
    </div>

</template>




<script>
import { normalizeProps } from 'vue';

export default {
    data() {
	return {
		num: 0,
		res: 0,
        number1:0,
        number2:0,
        resnumber: 0
	}
},
    methods: 
    {
        calc: function(){
        this.res = this.num ** 2
        },
        summ: function(){
            this.resnumber = this.number1 +  this.number2
        }
    }
}

</script>

<style>
@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');
</style>