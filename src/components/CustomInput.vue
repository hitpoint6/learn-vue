<script setup></script>

<template>
  <input
    type="text"
    placeholder="Custom Text Input"
    @change="$emit('customChange', $event.target.value)"
  />
</template>

<style></style>
