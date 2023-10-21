<script setup>
    import { ref } from 'vue'

    const source = ref('something.co');
</script>

<template>
    <div>
        <slot name="image">
            <img src="https://i.stack.imgur.com/y9DpT.jpg" />
        </slot>
        <slot name="caption" :source="source">Caption</slot>
    </div>
</template>

<style>
</style>