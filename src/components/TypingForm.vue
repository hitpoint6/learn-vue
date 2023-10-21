<script setup>
import { ref, watchEffect } from "vue";

const textContent = ref("");
const isTyping = ref(false);

const stop = watchEffect((onInvalidate) => {
  if (textContent.value.length > 0) {
    isTyping.value = true;

    if (textContent.value.length > 10) {
      stop();
    }

    const resetTyping = setTimeout(() => {
      isTyping.value = false;
    }, 2000);

    onInvalidate(() => {
      clearInterval(resetTyping);
    });
  }
});
</script>

<template>
  <textarea v-model="textContent"></textarea>
  <p v-if="isTyping">Kelvin is typing...</p>
</template>

<style></style>
