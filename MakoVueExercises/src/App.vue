
<template>
    <div class="withMargin"> 
        <div>
    <table>
      <thead>
        <tr>
          <th>ID</th>
          <th>Name</th>
          <th>Salary</th>
          <th>Age</th>
          <th>Actions</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="user in users" :key="user.id">
          <td>{{ user.id }}</td>
          <td>{{ user.name }}</td>
          <td>{{ user.salary }}</td>
          <td>{{ user.age }}</td>
          <td><button @click="removeUser(user.id)">Delete</button></td>
        </tr>
      </tbody>
    </table>
  </div>


        
    </div>



</template>

<script>
import { normalizeProps } from 'vue';

export default {
    data() {
	return {
		users: [
			{
				id: 1,
				name: 'Данил Ромашкан',
				salary: 100,
				age: 30,
                isEdit: false,
			},
			{
				id: 2,
				name: 'Давид Авагян',
				salary: 200,
				age: 40,
                isEdit: false,
			},
			{
				id: 3,
				name: 'Шагин Виталий',
				salary: 300,
				age: 50,
                isEdit: false,
			},
		],
	}
},
    methods: 
    {
    removeUser(id) {
    const index = this.users.findIndex(user => user.id === id)
    this.users.splice(index, 1)
    },
    }

}


</script>

<style>

@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');


</style>