<template>
	<div className="container">
      <h1 className="title">Welcome to Zillion Dollar Lottery!</h1>
      <p>You will submit this as your email address:</p>
      <Avatar />
	  <Input
	  	placeholder="Enter you email to win!"
		label="Email"
		v-bind:value="email" />
      
      <!-- Render message or input form -->
    </div>
</template>

<script>
import Avatar from "./components/Avatar";
import Input from "./components/Input";

export default {
	name: "LotteryForm",
	components: {
		Avatar,
		Input
	},
	data: () => {
		return {
			email: "andy@codechrysalis.io"
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
