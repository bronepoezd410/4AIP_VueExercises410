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
    one: function (name) {
      document.write(name)
    },
    two: function (name, salary) {
      document.write(name + '  ' + salary)
    }
  }
}
</script>




<template>

    <Rabotnik @show1="one" @show2="two"/>

</template>













<style>

@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');


</style>