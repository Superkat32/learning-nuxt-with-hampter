<script lang="ts">
import {ImgHampterVisual} from "#components";

export default {
  components: {
    ImgHampterVisual,
  }
}
</script>

<template>
  <div class="mx-8">
    <slot />
    <NuxtLink to="/">Take me home, Hampter!</NuxtLink>
  </div>
</template>