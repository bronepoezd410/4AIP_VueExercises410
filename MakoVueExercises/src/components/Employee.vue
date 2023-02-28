
<template>
	<template v-if="!isEdit">
	  <div>
		<h1>{{ name }}</h1>
		<h1>{{ surn }}</h1>
		<button @click="edit">edit</button>
	  </div>
	</template>
	<template v-else>
	  <div class="block">
		<input class="block_input" v-model="newName">
		<input class="block_input" v-model="newSurn">
		<button @click="save">save</button>
	  </div>
	</template>
  </template>

<script>
export default {
  props: {
    id: Number,
    name: String,
    surn: String,
  },
  emits: ['change'],
  data() {
    return {
      isEdit: false,
      newName: this.name,
      newSurn: this.surn,
    }
  },
  methods: {
    edit() {
      this.isEdit = true;
    },
    save() {
      this.isEdit = false;
      this.$emit('change', this.id, this.newName, this.newSurn);
    }
  }
}
</script>



// <!-- props: {
// 	title: String,
// 	likes: Number,
// 	isPublished: Boolean,
// 	commentIds: Array,
// 	author: Object,
// 	callback: Function,
// 	contactsPromise: Promise // или любой другой конструктор
// } -->