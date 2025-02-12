<template>
  <thetitle/>
  <tiersection :word="word1"/>
  <tiersection :word="word2"/>
  <tiersection :word="word3"/>
  <tierbar :t="tee"/>
  <tierdata :tierdata="test" />

  
</template>

<script setup>
  import thetitle from '@/components/thetitle.vue';
  import tiersection from '@/components/tiersection.vue';
  import tierdata from '@/components/tierchart.vue'
  import tierbar from '@/components/tierbar.vue';
  import buttons from '@/components/buttons.vue'
  const word1 = "word1"
  const word2 = "word2"
  const word3 = "word3"
  const tee = "tee"


  import { defineProps } from 'vue';
  const props = defineProps(["tierdata"])
</script>

<style scoped>

</style>