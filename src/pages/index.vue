<script setup lang="ts">
//
import { ref } from 'vue';

const maVar = ref(false)
console.log('maVar:', maVar.value)

</script>

<template>
  <button @pointerdown="maVar = true">Montrer</button>
  <button @pointerdown="maVar = false">Cacher</button>
  <h1 v-show="maVar" class="text-2xl">Bonjour toi !</h1>
</template>
