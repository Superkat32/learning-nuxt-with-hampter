<script setup lang="ts">
const props = defineProps<{
  variant?: "default" | "thinking" | "curious" | "happy" | "evil";
}>();

let hampterSource: string = "hampter.jpg";
switch (props.variant) {
  case "thinking": hampterSource = "faces/hampterThinking.png"; break;
  case "curious": hampterSource = "faces/hampterCurious.png"; break;
  case "happy": hampterSource = "faces/hampterHappy.png"; break;
  case "evil": hampterSource = "faces/hampterEvil.png"; break;
}
</script>

<template>
  <div>
    <NuxtImg
        :src="hampterSource"
        alt="Hampter"
        placeholder="/othonko.png"
    />
  </div>
</template>