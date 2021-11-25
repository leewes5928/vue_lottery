<template>
  <div class="container">
      <h1 class="title">Welcome to Zillion Dollar Lottery!</h1>
      <!-- this is where your HTML goes -->
    </div>
</template>

<script>
// TODO: Import child components

export default {
  name: 'LotteryForm',
  components: {
    // Child components here
  },
  data () {
    // State goes here
  }
}
</script>

<style scoped>
.title {
  font-size: 24px;
  color: teal;
}
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  width: 300px;
  margin: 20px auto;
  padding: 20px;
  border: 1px solid teal;
}
</style>
