<script setup>
import CustomInput from "./CustomInput.vue";

const logChange = (event) => {
  console.log(event);
};
</script>
<template>
  <CustomInput @customChange="logChange" />
</template>
