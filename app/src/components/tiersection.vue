

<script>
import { tierS, tierA, tierB, tierC, tierD, tierE, tierF } from "@/components/ALLTIERS.vue"








</script>

<template>

<div class="bar">
  <div class="tier-bar">
      <img class="img"v-for="(image, index) in tierS" :key="index" :src="image" alt="Tier Image"  />
    </div>
</div>

<div class="bar">
  <div class="tier-bar">
      <img class="img"v-for="(image, index) in tierA" :key="index" :src="image" alt="Tier Image"  />
    </div>
</div>

<div class="bar">
  <div class="tier-bar">
      <img class="img"v-for="(image, index) in tierB" :key="index" :src="image" alt="Tier Image"  />
    </div>
</div>

<div class="bar">
  <div class="tier-bar">
      <img class="img"v-for="(image, index) in tierC" :key="index" :src="image" alt="Tier Image"  />
    </div>
</div>

<div class="bar">
  <div class="tier-bar">
      <img class="img"v-for="(image, index) in tierD" :key="index" :src="image" alt="Tier Image"  />
    </div>
</div>

<div class="bar">
  <div class="tier-bar">
      <img class="img"v-for="(image, index) in tierE" :key="index" :src="image" alt="Tier Image"  />
    </div>
</div>

<div class="bar">
  <div class="tier-bar">
      <img class="img"v-for="(image, index) in tierF" :key="index" :src="image" alt="Tier Image"  />
    </div>
</div>


</template>

<style scoped>
.tier-bar {
  display: flex;
  gap: 10px;
  background-color: gray;
  padding: 10px;
  border-radius: 10px;
  min-height: 60px;
  align-items: center;
}

.img{
  width: 100%;
}
</style>