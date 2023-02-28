
<template>
    <AddUsers @add="add" />
  </template>
  
  


<script>
import AddUsers from './components/AddUsers.vue'
import Employee from './components/Employee.vue'

export default {
  components: {
    AddUsers, Employee
  },
  data() {
    return {
      users: [
        {
          id: 1,
          name: 'name1',
          surn: 'surn1'
        },
        {
          id: 2,
          name: 'name2',
          surn: 'surn2'
        },
        {
          id: 3,
          name: 'name3',
          surn: 'surn3'
        },
      ],
    }
  },
  methods: {
    add(name, surn) {
      let id = this.users.length + 1;
      this.users.push({id, name, surn});
      console.log(this.users)
    }
  }
}
</script>


<style>

@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');


</style>