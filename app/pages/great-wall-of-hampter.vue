<script setup lang="ts">
let hampterCount: number = 50;
</script>

<template>
  <div>
    <h1>Welcome to The Great Wall of Hampter</h1>

  </div>
  <div class="grid grid-cols-7 gap-1">
    <div v-for="unused in hampterCount">
      <ImgHampterVisual />
    </div>
  </div>
</template>