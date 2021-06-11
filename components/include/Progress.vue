<template>
  <div>
    <div>
      <b-progress :value="value" :max="max" show-progress animated></b-progress>
      <b-progress class="mt-2" :max="max" show-value>
        <b-progress-bar
          :value="value * (6 / 10)"
          variant="success"
        ></b-progress-bar>
        <b-progress-bar
          :value="value * (2.5 / 10)"
          variant="warning"
        ></b-progress-bar>
        <b-progress-bar
          :value="value * (1.5 / 10)"
          variant="danger"
        ></b-progress-bar>
      </b-progress>

      <b-button class="mt-3" @click="randomValue">Click me</b-button>
    </div>
    <br>
    <div>
      <b-progress :value="value1" :max="max1" class="mb-3"></b-progress>
      <b-progress :value="value1" :max="max1" show-value class="mb-3"></b-progress>
      <b-progress :value="value1" :max="max1" show-progress class="mb-3"></b-progress>
      <b-progress :value="value1" :max="max1" :precision="2" show-value class="mb-3"></b-progress>
      <b-progress :value="value1" :max="max1" :precision="2" show-progress class="mb-3"></b-progress>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      value: 45,
      max: 100,
      value1: 33.333333333,
      max1: 50
    }
  },
  methods: {
    randomValue() {
      this.value = Math.random() * this.max
    },
  },
}
</script>
