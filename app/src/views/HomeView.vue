<template>
  <thetitle/>
  <img class="images" v-if="listofimages.length" :src="listofimages[0]" alt="">
  <p v-if="!listofimages.length">no more images</p>
  <div>
    <button @click="cycleS">s</button>
    <button @click="cycleA">a</button>
    <button @click="cycleB">b</button>
    <button @click="cycleC">c</button>
    <button @click="cycleD">d</button>
    <button @click="cycleE">e</button>
    <button @click="cycleF">f</button>
  </div>

  <TierChart/>
</template>

<script setup>
import TierChart from '@/components/tiersection.vue'
import { listofimages } from '@/components/image.vue';
import thetitle from '@/components/thetitle.vue';
import { cycleS, cycleA, cycleB, cycleC, cycleD, cycleE, cycleF } from '@/components/buttontiers.vue';
</script>

<style scoped>
p{
  font-size: 30px;
}

button{
  font-size: 30px;
}

.images{
  width: 25%;
  height: 400px;
}
</style>
