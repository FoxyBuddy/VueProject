<template>
  <LoginForm></LoginForm>
</template>

<script>
import LoginForm from './LoginForm.vue'
export default {
  components: {
    LoginForm
  },
  name: 'my-first-vue',
  data: function () {
    return {
      serverResponse: 'resp',
      niebaoni: 'nbsps'
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
