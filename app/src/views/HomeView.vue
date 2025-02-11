<template>
  <thetitle/>
  <tiersection :word="word1"/>
  <tiersection :word="word2"/>
  <tiersection :word="word3"/>
</template>

<script setup>
  import thetitle from '@/components/thetitle.vue';
  import tiersection from '@/components/tiersection.vue';
  const word1 = "word1"
  const word2 = "word2"
  const word3 = "word3"
</script>

<style scoped>

</style>