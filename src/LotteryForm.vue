<template>
  <div class="container">
      <h1 class="title">{{title}}</h1>
      <!-- this is where your HTML goes -->
      <Avatar />
      <Input placeholder="Enter email to win!" label-text="Email"/>
      <Submit @myclick="handleClick" />
    </div>
</template>

<script>
// TODO: Import child components
import Avatar from './components/Avatar.vue'
import Input from './components/Input.vue'
import Submit from './components/Submit.vue'

export default {
  name: 'LotteryForm',
  components: {
    // Child components here
    Avatar,
    Input,
    Submit
  },
  data () {
    // State goes here
    return {
      title: 'Welcome to Zillion Dollar Lottery!'
    }
  },
  methods: {
    handleClick: function (data) {
      console.log(data)
    }
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
