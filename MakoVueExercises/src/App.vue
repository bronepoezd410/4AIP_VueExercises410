<template>
    <div>
        {{ count }}
        <p>Hello, World!</p>
        <p>{{ text1 }}</p>
        <p>{{ text2 }}</p>
        <p>{{ text3 }}</p>
    </div>


    <div> {{ name }} </div>

    <div>{{ surn }}</div>
</template>


<script>
export default {
    name: 'App',

     data() {
        return{
            text1: 'Предложение номер 1',
            text2: 'Предложение номер 2',
            text3: 'Предложение номер 3',
            count: 0,
            name: 'Makosin',
		    surn: 'Dzjaszchkowiczh',
        }
    }
}
</script>

<style>

</style>