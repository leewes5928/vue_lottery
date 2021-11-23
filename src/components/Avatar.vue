<template>
  <div class="avatar">
    <img class="avatar" v-bind:src="image" alt="" />
  </div>
</template>

<script>
export default {
  name: 'Avatar',
  data () {
    return {
      image: ''
    }
  },
  mounted () {
    fetch('https://source.unsplash.com/random').then(
      (response) => {
        this.image = response.url
      }
    )
  }
}
</script>

<style scoped>
  .avatar {
    width: 200px;
    height: 200px;
    border-radius: 50%;
    margin: 20px;
    object-fit: cover;
  }
</style>
