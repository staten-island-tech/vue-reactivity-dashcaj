<template>
  <thetitle/>
  <p v-if="listofimages.length">{{ "Image " + listofimages[0] }}</p>
  <p v-if="!listofimages.length">no more images</p>
  <div>
    <button @click="cycle">s+</button>
    <button @click="cycle">a</button>
    <button @click="cycle">b</button>
    <button @click="cycle">c</button>
    <button @click="cycle">d</button>
    <button @click="cycle">e</button>
    <button @click="cycle">f</button>
  </div>

</template>

<script setup>
  import thetitle from '@/components/thetitle.vue';
  import tiersection from '@/components/tiersection.vue';
  import tierdata from '@/components/tierchart.vue'
  import {listofimages, cycle} from '@/components/image.vue'

  import { defineProps } from 'vue';
  const props = defineProps(["tierdata"])
</script>

<style scoped>
p{
  font-size: 30px;
}

button{
  font-size: 30px;
}
</style>