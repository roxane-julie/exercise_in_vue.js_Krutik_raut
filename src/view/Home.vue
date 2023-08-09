<template>
  <Hello/>
 
</template>

<script setup>
import Hello from '../components/Hello.vue'
import InfosCounter from '../components/InfosCounter.vue'

import { onMounted } from 'vue';

onMounted(async()=>{

  // fetch('https://jsonplaceholder.typicode.com/posts')
  // .then((response) =>response.json())
  // .then((data) =>{
  //   console.log(data);
  // })

  let data = await fetch('https://jsonplaceholder.typicode.com/posts');
  data = data.json()
  console.log(await data)
}
)
</script>

<style>
</style>