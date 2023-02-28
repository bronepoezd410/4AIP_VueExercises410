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
  methods: {
    showApp1: function () {
      this.$emit('show1', 'Давид Авагян');
    },
    showApp2: function () {
      this.$emit('show2', 'Давид Авагян', '5$');
    }
  }
}
</script>

<template>
	  <button @click="showApp1">Первое </button>
	  <button @click="showApp2">Второе </button>
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