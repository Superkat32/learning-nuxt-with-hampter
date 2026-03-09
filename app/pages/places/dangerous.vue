<script setup lang="ts">
definePageMeta({
  layout: "somewhere"
})
</script>

<template>
  <h1>Dangerous !</h1>
  <ImgHampterVisual variant="evil" />
  <div class="my-2">
    <span>This Hampter is</span>
    <span class="
      inline-block text-white bg-red-700 rounded-md
      mx-0.5 px-0.5 py-0
      animate-shake transition delay-25 duration-300 ease-in-out hover:animate-shake-more hover:scale-110 hover:bg-red-500"
    >EVIL</span>
    <span>!!</span>
  </div>
</template>