<template>
  <div class="container">
    <div>
      <Logo />
      <h1 class="title">Post_ID: {{ $route.params.PostID }}</h1>
      <LinkNuxt />
    </div>
  </div>
</template>
<script>
import Custom from '@/components/style/custom.vue'
export default {
  components: {
  },
  validate(data) {
    return /^\d+$/.test(data.params.PostID)
  },
}
</script>
