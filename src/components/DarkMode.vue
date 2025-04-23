<script setup>
import { useDark, useToggle } from "@vueuse/core";

const isDark = useDark();
const toggleDark = useToggle(isDark);
</script>

<template>
  <p>Dark theme: {{isDark}}</p>

  <button @click="toggleDark()">
    Toggle Color Mode
  </button>
</template>

<style>
.dark {
  background: #16171d; 
  color: #fff;
}
</style>