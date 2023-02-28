

<template>
	<Rabotnik :name="[1, 2, 3]" />
</template>





<script>
import Rabotnik from './components/Employee.vue'
export default {
  components: {
    Rabotnik
  }
}
</script>

<style>

@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');


</style>