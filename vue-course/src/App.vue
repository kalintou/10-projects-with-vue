<script setup>
import FromComponent from './components/FromComponent.vue'

const formHander = (username, email, password) => {
  console.log('username', username)
  console.log('email',email)
  console.log('password', password)
}

</script>


<template>
  <FromComponent @userInfo="formHander"/>
</template>
