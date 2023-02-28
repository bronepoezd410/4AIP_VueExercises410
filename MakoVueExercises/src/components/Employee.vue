<script>
export default {
  props: {
    id: Number,
    name: String,
    surn: String,
  },
  emits: ['remove'],
  data() {
    return {
    }
  },
}
</script>

<template>
  <div class="block">
    {{ name }}
    {{ surn }}
    <button class="btn" @click="$emit('remove', id)">remove</button>
  </div>
  
</template>


// <!-- props: {
// 	title: String,
// 	likes: Number,
// 	isPublished: Boolean,
// 	commentIds: Array,
// 	author: Object,
// 	callback: Function,
// 	contactsPromise: Promise // или любой другой конструктор
// } -->