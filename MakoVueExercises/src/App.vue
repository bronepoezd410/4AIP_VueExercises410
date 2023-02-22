
<template>
    <div class="withMargin"> 
    <p>
        Какой язык для вас родной?
    </p>
    <input name="radio" type="radio" v-model="choice" value="Русский"> Русский
	<input name="radio" type="radio" v-model="choice" value="Немецкий"> Немецкий
	<input name="radio" type="radio" v-model="choice" value="Английский"> Английский
    <br>

    you choosed: {{ choice }}

    <p v-if="choice == 'Русский'">
        Россия — священная наша держава, 
        Россия — любимая наша страна.
        Могучая воля, великая слава —
        Твоё достоянье на все времена!
        Славься, Отечество наше свободное,
        Братских народов союз вековой,
        Предками данная мудрость народная!
        Славься, страна! Мы гордимся тобой!</p>
    <p v-if="choice == 'Немецкий'">
        Einigkeit und Recht und Freiheit
        für das deutsche Vaterland!
        Danach lasst uns alle streben
        brüderlich mit Herz und Hand!
        Einigkeit und Recht und Freiheit
        sind des Glückes Unterpfand!
        Blüh im Glanze dieses Glückes,
        blühe, deutsches Vaterland!
        Blüh im Glanze dieses Glückes,
        blühe, deutsches Vaterland!</p>
    <p v-if="choice == 'Английский'">
        God save our gracious King (Queen)!
        Long live our noble King (Queen)!
        God save the King (Queen)!s
        Send him (her) victorious,
        Happy and glorious,
        Long to reign over us:
        God save the King (Queen).</p>



    </div>


</template>

<script>
//import { normalizeProps } from 'vue';

export default {
    data() {
        return {
            choice: '',
        	}
},
    methods: 
    {

    }
}


</script>

<style>

@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');


</style>