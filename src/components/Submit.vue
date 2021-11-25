<template>
  <button @click="onClicker">Submit</button>
</template>

<script>
export default {
  name: 'Submit',
  methods: {
    onClicker: function (e) {
      this.$emit('myclick', 'data')
      console.log('clicked')
    }
  },
  emits: ['myclick']
}
</script>

<style scoped>
.button {
  border-radius: 5px;
  padding: 15px;
  width: 200px;
  background-color: transparent;
}
.button:hover {
  cursor: pointer;
  background-color: teal;
  color: white;
}
</style>
