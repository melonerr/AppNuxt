<template>
  <div>
    <Nuxt />
  </div>
</template>

<script>

export default {

  methods: {
    showDropDownMenu() {
      var element = document.getElementById('navbarNavAltMarkup')
      element.classList.toggle('collapse')
    },
  },
}
</script>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.button--success {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #218838;
  color: #218838;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 8px;
}

.button--success:hover {
  color: #fff;
  background-color: #28a745;
}

.button--secondary {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #5a6268;
  color: #5a6268;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 8px;
}

.button--secondary:hover {
  color: #fff;
  background-color: #6c757d;
}

.button--primary {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #0069d9;
  color: #0069d9;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 8px;
}

.button--primary:hover {
  color: #fff;
  background-color: #007bff;
}

.button--info {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #138496;
  color: #138496;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 8px;
}

.button--info:hover {
  color: #fff;
  background-color: #17a2b8;
}

.button--danger {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #c82333;
  color: #c82333;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 8px;
}

.button--danger:hover {
  color: #fff;
  background-color: #dc3545;
}

.button--warning {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #e0a800;
  color: #e0a800;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 8px;
}

.button--warning:hover {
  color: #fff;
  background-color: #ffc107;
}

.button--light {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #f8f9fa;
  color: #f8f9fa;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 8px;
}

.button--light:hover {
  color: #fff;
  background-color: #e2e6ea;
}
.button--dark {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #343a40;
  color: #343a40;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 8px;
}

.button--dark:hover {
  color: #fff;
  background-color: #23272b;
}

.box-shadow {
  box-shadow: 0 0 18px 0 rgb(0 0 0 / 33%);
}
.bg-white {
  background-color: white;
}

.p-lr-5 {
  padding: 0rem 1rem !important;
}
</style>
