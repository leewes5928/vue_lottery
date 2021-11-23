<template>
	<div>
      <label v-bind:for="label">{{labelName}}</label>
      <input class="input"
        v-bind:value="value"
        v-bind:placeholder="placeholder"
      />
    </div>
</template>

<script>
export default {
	name: "Input",
	props: ['labelName', 'value', 'placeholder']
}
</script>

<style scoped>
.input {
	display: flex;
	flex-direction: column;
	font-size: 18px;
	margin: 20px 0;
	padding: 5px;
}
</style>
