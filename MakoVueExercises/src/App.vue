
<template>
    <button @click="delogin"> {{ isAuth ? 'hide' : 'show' }}</button>
		<p v-if="isAuth">+++</p>

    <p> v-if осуществляет фактическую отрисовку, при false уничтожает объект и появляется он сам только в моменте обращения результата условия в true, лучше всего использовать когда элементы будут нечасто переключены </p>
    <p> v-show осуществляет отрисовку заранее и появляется/исчезает внешне но всегда создан, лучше всего использовать при частом взаимодействии с объектом. Директиву v-show нельзя использовать на элементе template и она не работает с v-else. </p>
</template>

<script>
import { normalizeProps } from 'vue';

export default {
    data() {
	return {
        isAuth: true,
	}
},
    methods: 
    {
        delogin: function(){
            this.isAuth = !this.isAuth
        },
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