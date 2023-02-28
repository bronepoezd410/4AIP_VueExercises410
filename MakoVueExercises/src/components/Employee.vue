
<template>
	<div class="withMargin">
	  <button @click="$emit('show1')">One</button>
	  <button @click="$emit('show2')">Two</button>
	</div>
  </template>

<script>
export default {
  props: {
    show1: Number,
    show2: Number,
  },
  data() {
    return {
    }
  },
  
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