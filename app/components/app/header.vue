<script setup lang="ts">
const props = defineProps<{
  showTitle?: boolean
}>();

let showTitle: boolean = props.showTitle; // Default to true, otherwise use props.showTitle value
</script>

<template>
  <header>
    <div class="mt-1 mb-4">
      <nav class="border-b-1 pb-1 border-gray-300">
        <div class="flex justify-between">
          <ul class="flex flex-row gap-x-2">
            <li class="navbar-link">
              <NuxtLink to="/" class="text-white no-underline">Home</NuxtLink>
            </li>

            <li class="navbar-link">
              <NuxtLink :to="{ name:'great-wall-of-hampter' }" class="text-white no-underline">Great Wall of Hampter</NuxtLink>
            </li>

          </ul>
          <ul class="flex flex-row gap-x-2">
            <li class="navbar-link">
              <NuxtLink :to="{ name:'about' }" class="text-white no-underline">About</NuxtLink>
            </li>
          </ul>
        </div>
        <div v-if="showTitle">
          <h1 class="text-5xl font-bold flex justify-center">Learning Nuxt with Hampter!</h1>
          <p class="text-xl font-medium flex justify-center">Hampter!</p>
        </div>
      </nav>
    </div>
  </header>
</template>