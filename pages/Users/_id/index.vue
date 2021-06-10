<template>
  <div class="container">
    <div>
      <Logo />
      <h1 class="title">User_id: {{ $route.params.id }}</h1>
      <LinkNuxt />
    </div>
  </div>
</template>

<script>
import Custom from '@/components/style/custom.vue'
export default {
  validate(data) {
    return /^\d+$/.test(data.params.id)
  },
}
</script>
