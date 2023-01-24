<template>
  <form action="/Register" method="post" @submit.prevent>
    <input v-model="username" type="text" maxlength="10" placeholder="请输入用户名"/> <br />
    <input v-model="password" type="password" maxlength="10" placeholder="请输入登录密码"/> <br />
    <input v-model="identifyNO" type="text" maxlength="10" placeholder="请输入管理员的ID号"/> <br />
    <p>输入的用户名：{{this.username}}</p>
    <p>输入的密码：{{this.password}}</p>
    <p>输入的ID号：{{this.identifyNO}}</p>
    <SQLRequest />
  </form>
</template>

<script>
import SQLRequest from './SQL_request.vue'
export default {
  components: {
    SQLRequest
  },
  name: 'LoginForm',
  data () {
    return {
      username: '',
      password: '',
      identifyNO: 0
    }
  }
}
</script>

<style scoped>
 input[type="text"]{
   border: 1px solid rgba(124, 255, 255, 1.0);
 }
</style>
