<template>

    <div>
    <select v-model="selected">
        <option>1</option>
        <option>2</option>
        <option>3</option>     
        <option>4</option>     
        <option>5</option>     
        <option>6</option>     
        <option>7</option>      
    </select>
        <p><span>Номер дня недели по счету: {{selected}} </span></p>
        <button @click="show">Показать название дня</button>
    </div>

</template>


<script>
import { normalizeProps } from 'vue';

export default {
    data() {
	    return {
            selected: 'Не выбрано ',
	    }
    },
	methods: {
	show: function() {
		let selected1 = this.cape(this.selected);
		alert('Выбранный день по счету это ' + selected1);
        
        let date = new Date();
        let dayWeek = ['7', '1', '2', '3', '4', '5', '6'][date.getDay()];
        alert('А сегодня - ' + this.cape(dayWeek)); 
	},

	cape: function(day_number) {
		switch (day_number) {
            case '1':
                return (day_number = 'Понедельник')
                break
            case '2':
                return (day_number = 'Вторник')
                break
            case '3':
                return (day_number = 'Среда')                
                break
            case '4':
                return (day_number = 'Четверг')
                break
            case '5':
                return (day_number = 'Пятница')
                break
            case '6':
                return (day_number = 'Суббота')
                break
            case '7':
                return (day_number = 'Воскресенье')
                break
            // default:
            //     return (day_number = 'У меня нет ответа для тебя')
        }
        }
	}
	}

</script>

<style>

</style>