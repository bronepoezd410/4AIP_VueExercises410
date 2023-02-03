<template>
    <div>
        Hello, World!
        <!-- Количество: {{ count }} -->
        <h1> Написать какой-нибудь текст с тегами</h1>
        <b> Написать какой-нибудь текст с тегами</b>
        <h2> Написать какой-нибудь текст с тегами</h2>
        <b> </b>
    </div>
</template>


<script>
export default {
    name: 'App',

     data() {
        return{
            count: 0,
        }
    }
}
</script>


<style>

</style>