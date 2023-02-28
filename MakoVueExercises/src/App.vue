<script>
import Rabotnik from './components/Employee.vue'
export default {
  components: {
    Rabotnik
  },
  data() {
    return {
      users: [
        {
          id: 1,
          name: 'Давид',
          surn: 'Авагян'
        },
        {
          id: 2,
          name: 'Данил',
          surn: 'Ромашкан'
        },
        {
          id: 3,
          name: 'Виталий',
          surn: 'Шагин'
        },
      ],
    }
  },
  methods: {
    remove(id) {
      this.users = this.users.filter((user) => {
        return user.id !== id;
      })
    }
  }
}
</script>

<template>
  <Rabotnik
		v-for="user in users"
		:id="user.id"
		:name="user.name"
		:surn="user.surn"
		@remove="remove"
		:key="user.id"
	/>
</template>











<style>

@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');


</style>