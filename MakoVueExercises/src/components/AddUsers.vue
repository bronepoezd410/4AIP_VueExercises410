<template>
    <div>
       <input class="block_input" v-model="newName">
       <input class="block_input" v-model="newSurn">
       <button @click="save">Save</button>
    </div>
 </template>




<script>
export default {
   data() {
      return {
         newName: ' ',
         newSurn: ' ',
      }
   },
   methods: {
      save() {
         this.$emit('add', this.newName, this.newSurn)
      }
   }
}
</script>

