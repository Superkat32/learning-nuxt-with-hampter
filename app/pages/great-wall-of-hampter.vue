<script setup lang="ts">
const monthDays: number[] = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]

const date: Date = new Date();
let month: number = date.getMonth();
let monthDate: number = date.getDate();

// I can't believe I got this first try
let hampterCount: number = 0;
for (let i = 0; i < month; i++) {
  hampterCount += monthDays[i] || 0;
}
hampterCount += monthDate;

</script>

<template>
  <div>
    <h1>Welcome to The Great Wall of Hampter</h1>
    <p>After every day during the year, a new Hampter is added, increasing the ever-growing Great Wall of Hampter.</p>
    <span>There are currently</span> <span class="inline-block text-white bg-blue-400 rounded-md mb-0.5 px-0.5 py-0">{{ hampterCount }} Hampters</span>
  </div>
  <div class="grid grid-cols-7 gap-1">
    <div v-for="unused in hampterCount">
      <ImgHampterVisual />
    </div>
  </div>
</template>