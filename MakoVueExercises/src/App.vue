<template>

<div>
    <table>
      <thead>
        <tr>
          <th>ID</th>
          <th>Name</th> 
          <th>Surname</th> 
        </tr>
      </thead>
      <tbody>
        <tr v-for="user in users" :key="user.id">
        <template v-if="!user.isEdit">
          <td>{{ user.id }}</td>
          <td>{{ user.name }}</td>
          <td>{{ user.surn }}</td>
          <button @click="edit(user)"> edit </button>
        </template>
        <template v-else>
                <td>{{ user.id }}</td>
				<td> <input v-model="user.name"> </td>
				<td>  <input v-model="user.surn"> </td>
                <td>  <button @click="save(user)">save</button></td>
			</template>
        </tr>
      </tbody>
    </table>
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
				name: 'name1',
				surn: 'surn1',
				isEdit: false,
			},
			{
				id: 2,
				name: 'name2',
				surn: 'surn2',
				isEdit: false,
			},
			{
				id: 3,
				name: 'name3',
				surn: 'surn3',
				isEdit: false,
			},
		]
	}
},
    methods: 
    {
        edit(user) {
		user.isEdit = true;
	},
	    save(user) {
		user.isEdit = false;
	},
    }

}


</script>

<style>

@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');


</style>