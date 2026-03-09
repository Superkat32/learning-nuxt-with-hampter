<script lang="ts">
import {AppHeader, ImgHampterVisual} from "#components";

export default {
  components: {
    ImgHampterVisual,
    AppHeader,
  }
}
</script>

<template>
  <div class="mx-8">
    <AppHeader />
    <slot />
    <NuxtLink to="/">Take me home, Hampter!</NuxtLink>
  </div>
</template>