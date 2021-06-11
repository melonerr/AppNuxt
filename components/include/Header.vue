<template>
  <div class="Header">
    <nav
      class="
        navbar navbar-expand-lg navbar-light
        bg-light
        box-shadow
        bg-white
        sticky-top
      "
    >
      <div class="container-fluid">
        <a class="navbar-brand">
          <img src="~assets/img/jrdream-logo.png" width="40px" />
        </a>
        <button
          class="navbar-toggler"
          type="button"
          @click.prevent="showDropDownMenu"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
          <div class="navbar-nav">
            <a class="nav-link active" aria-current="page">Home</a>
            <a class="nav-link">Features</a>
            <a class="nav-link">Pricing</a>
            <a class="nav-link disabled" tabindex="-1" aria-disabled="true"
              >Disabled</a
            >
          </div>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style scoped>
</style>
