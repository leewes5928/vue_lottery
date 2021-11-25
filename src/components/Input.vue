<template>
  <label>
    {{labelText}}
    <input type="email" :placeholder="placeholder" />
  </label>
</template>

<script>
export default {
  name: 'Input',
  props: ['placeholder', 'labelText']
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
