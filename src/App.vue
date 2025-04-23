<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import DarkMode from '@/components/DarkMode.vue';
</script>

<template>
  
<DarkMode />
<RouterView />
</template>

<style scoped>
  body {
    background-image: url('https://images7.alphacoders.com/716/716405.jpg');
    background-size: cover;
    background-position: center;
    height: 100vh;
    margin: 0;
  }
  .naam{
    font-weight: bold;
  }
  .naam:hover .naam_icons{
    display: block;
    transform: scale(1.2);
    rotate: 10deg;
  }
  .naam:hover .naam_letter{
    display: none;
  }
  .naam_icons{
    display: none;
  }

  #content{
    height: 300vh;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
  }
  #div1{
    height: 92vh;
    background-color: red;
    display: grid;
    grid-template-rows: repeat(2, 1fr);
  }
  #div1a{
    padding: 20px;
    background-color: salmon;
  }
  #div1b{
    padding: 20px;
    background-color: darkred;
  }

  #div2{
    height: 100vh;
    background-color: blue;
  }
  #div3{
    height: 100vh;
    background-color: green;
  }
</style>