<template>
  <div class="links">
    <nuxt-link class="button--primary text-decoration" to="/" >Home</nuxt-link>
    <nuxt-link class="button--success text-decoration" to="/admin" >Admin</nuxt-link>
    <nuxt-link class="button--warning text-decoration" to="/posts" >Posts</nuxt-link>
    <br><br>
    <nuxt-link class="button--info text-decoration" to="/users" >User</nuxt-link>
    <nuxt-link class="button--danger text-decoration" to="/" target="_blank" >_Blank</nuxt-link>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.text-decoration{
  text-decoration:none
}
</style>
