<script setup lang="ts">
import { onMounted, ref } from "vue";
import WatermelonJSON from "./assets/watermelon.json";

let anim = ref();

onMounted(() => {
  setTimeout(() => {
    anim.value;
  }, 500);
});
</script>

<template>
  <lottie-animation
    :animation-data="WatermelonJSON"
    :auto-play="true"
    :loop="true"
    :speed="1"
    ref="anim"
  />
</template>

<style></style>
