<template>
<p>{{ t }}</p>

</template>

<script setup>
import { defineProps } from 'vue';
const props = defineProps(["t"])
</script>