<template>
  <ImgHampterVisual variant="default"/>

  <p>How will Hampter decide your fate today?</p>
  <ul>
    <li><NuxtLink :to="{ name: 'places-happy' }">Take me somewhere happy...</NuxtLink></li>
    <li><NuxtLink :to="{ name: 'places-exciting' }">Take me somewhere exciting...</NuxtLink></li>
    <li><NuxtLink :to="{ name: 'places-curious' }">Take me somewhere curious...</NuxtLink></li>
    <li><NuxtLink :to="{ name: 'places-dangerous' }">Take me somewhere dangerous...</NuxtLink></li>
  </ul>
</template>