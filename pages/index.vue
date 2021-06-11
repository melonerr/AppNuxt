<template>
  <div>
    <div class="container-fluid pl-0 pr-0">
      <Carousel />
    </div>
    <div class="container">
      <div>
        <Logo />
        <h1 class="title text-upper">Home</h1>
        <LinkNuxt />
      </div>
    </div>
  </div>
</template>

<script>
import Custom from '@/components/style/custom.vue'
import Carousel from '/components/include/Carousel.vue'
export default {
  components: {
    Carousel,
  },
}
</script>
