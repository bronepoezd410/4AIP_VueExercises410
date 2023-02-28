



<template>

    <Rabotnik @show1="one" @show2="two"/>

</template>



<script>
import Rabotnik from './components/Employee.vue'

export default {
  components: {
    Rabotnik
  },

  data() {
	return {
	}
},
methods: {
    one: function () {
      document.write('Сообщение 1')
    },
    two: function () {
      document.write('Сообщение 2')
    }
}
}
</script>















<style>

@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');


</style>