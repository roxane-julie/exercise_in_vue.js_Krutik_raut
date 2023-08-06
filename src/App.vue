
<template>
  <Header/>
  <RouterView/>
</template>


<script setup>
import { RouterView } from "vue-router";
import Header from "../src/components/Header.vue"




</script>


<style>

@font-face {
  font-family: 'poppins';
  src: url('../src/assets/Poppins-Light.ttf');
}
@font-face {
  font-family: 'poppins-bold';
  src: url('../src/assets/Poppins-Bold.ttf');
}
@font-face {
  font-family: 'poppins-semi-bold';
  src: url('../src/assets/Poppins-SemiBold.ttf');
}

</style>
