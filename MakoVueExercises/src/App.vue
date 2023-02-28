

<template>
<Rabotnik v-for="user in users"
		:id="user.id"
		:name="user.name"
		:surn="user.surn"
		:key="user.id"
    @change="change"
/>
</template>



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
          name: 'Эдем',
          surn: 'Османов'
        },
      ],
    }
  },
  methods: {
    change(id, name, surn){
      this.users = this.users.map((user) => {
        if(user.id === id){
          user.name = name;
          user.surn = surn;
        }
        return user;
      });
    }
  }
}
</script>








<style>

@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');


</style>