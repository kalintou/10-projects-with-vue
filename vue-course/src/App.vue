<script setup>
import {ref} from 'vue'
const firstName = ref('HuXn')
const lastName = ref('WebDev')
const myFavoriteNumber = ref(7)

import StaticPropsComponents from './components/StaticPropsComponents.vue';
import DynamicPropsComponent from './components/DynamicPropsComponent.vue';
import ChangingPropsValue from './components/ChangingPropsValue.vue';
import PropValidation from './components/PropValidation.vue';
import ComplexProps from './components/ComplexProps.vue';
import CustomValidator from './components/CustomValidator.vue';
</script>


<template>
  <!-- <StaticPropsComponents name="Jordan"/>
  <hr>
  <DynamicPropsComponent :firstName="firstName" :lastName="lastName"/>
  <hr>
  <ChangingPropsValue :myFavoriteNumber="myFavoriteNumber"/>
  <hr>
  <PropValidation fullName="HuXn WebDev" :age="20"/>
  <hr>
  <ComplexProps 
    :friends="['alex','john','kan','johnson']" 
    :userInfo="{name: 'alex', age: 20, location: ['Earth', 'IDK']}"
  />
  <hr> -->
  <CustomValidator name="Kan" :age="20" password="12345678password"/>
  <hr>
</template>
