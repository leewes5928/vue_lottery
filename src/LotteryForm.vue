<template>
  <div class="container">
      <h1 class="title">Welcome to Zillion Dollar Lottery!</h1>
      <Avatar />
      <p>You will submit this as your email address:</p>
    <Input
      placeholder="Enter you email to win!"
    labelName="Email"
    v-bind:value="email" />
      
      <Submit />
    </div>
</template>

<script>
import Avatar from './components/Avatar'
import Input from './components/Input"'
import Submit from './components/Submit'

export default {
  name: 'LotteryForm',
  components: {
    Avatar,
    Input,
    Submit
  },
  data () {
    return {
      email: 'andy@codechrysalis.io'
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
