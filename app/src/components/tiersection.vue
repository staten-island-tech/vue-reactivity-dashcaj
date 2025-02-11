<template>
<p>{{ word }}</p>


</template>

<script setup>

    import { defineProps } from 'vue';
    const props = defineProps(["word"])
</script>