<template>

    <Rabotnik :name="name" :salary="salary" :age="age"/>



</template>


<script>
import Rabotnik from './components/Employee.vue'


export default {
  components: {
    Rabotnik
  },


  data() {
	return {
      name: 'Давид Авагян',
      salary: '5$',
      age: '20',
	}
}
}
</script>

<style>

@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');


</style>