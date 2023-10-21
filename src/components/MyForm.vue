<script setup>
import { ref, onMounted } from "vue";

const name = ref("");

const el = ref();

const submitForm = () => {
  console.log(`Form submitted! Name = ${name.value}`);
};

onMounted(() => {
  el.value.focus();
});
</script>

<template>
  <p>{{ name }}</p>
  <input ref="el" type="text" placeholder="Name" v-model="name" />
  <div>
    <button @click="submitForm" :disabled="name.length == 0">Submit</button>'
  </div>
</template>

<style>
input[type="text"] {
  padding: 5px;
}

button {
  margin-top: 20px;
}
</style>
