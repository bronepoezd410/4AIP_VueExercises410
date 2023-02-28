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
    Name(name) {
        console.log(name);
    },
    Salary(salary){
        console.log(salary);
    }
  }
}
</script>




<template>
    <Rabotnik @show="Name" @show1="Salary"/>
</template>













<style>

@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');


</style>