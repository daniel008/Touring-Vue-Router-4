<template>
  <h1>Oops!</h1>
  <h3>The {{ resource }} you're looking for is not here.</h3>
  <router-link class="go-back-link" :to="{ name: 'EventList' }"
    >Back to the home page</router-link
  >
</template>

<script>
export default {
  props: {
    resource: {
      type: String,
      required: true,
      default: 'page'
    }
  }
}
</script>

<style scoped>
.go-back-link {
  color: #2c3e50;
  cursor: pointer;
}
</style>
