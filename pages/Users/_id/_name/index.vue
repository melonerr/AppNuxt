<template>
  <div class="container">
    <div>
      <Logo />
      <h1 class="title">
        User_id: {{ $route.params.id }} <br>
        User_name: {{ $route.params.name }}
      </h1>
      <LinkNuxt />
    </div>
  </div>
</template>

<script>
import Custom from '@/components/style/custom.vue'
export default {}
</script>
