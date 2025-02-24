

<script>
import { tiers } from '@/components/ALLTIERS.vue'


export default {
  data() {
    return {
      tiers,
    }
  },
}





</script>

<template>






<div class="bar"  id="s">
    <h1 class="labels">S</h1>
    <div class="tier-bar">
      <img class="img" v-for="image in tiers.tierS" :key="image" :src="image" alt="Tier Image" />
    </div>
</div>


<div class="bar">
  <h1 class="labela">A</h1>
    <div class="tier-bar">
      <img class="img" v-for="image in tiers.tierA" :key="image" :src="image" alt="Tier Image" />
    </div>
</div>


<div class="bar">
  <h1 class="labelb">B</h1>
    <div class="tier-bar">
      <img class="img" v-for="image in tiers.tierB" :key="image" :src="image" alt="Tier Image" />
    </div>
</div>


<div class="bar">
  <h1 class="labelc">C</h1>
    <div class="tier-bar">
      <img class="img" v-for="image in tiers.tierC" :key="image" :src="image" alt="Tier Image" />
    </div>
</div>


<div class="bar">
  <h1 class="labeld">D</h1>
    <div class="tier-bar">
      <img class="img" v-for="image in tiers.tierD" :key="image" :src="image" alt="Tier Image" />
    </div>
</div>



<div class="bar">
  <h1 class="labele">E</h1>
    <div class="tier-bar">
      <img class="img" v-for="image in tiers.tierE" :key="image" :src="image" alt="Tier Image" />
    </div>
</div>



<div class="bar">
  <h1 class="labelf">F</h1>
    <div class="tier-bar">
      <img class="img" v-for="image in tiers.tierF" :key="image" :src="image" alt="Tier Image" />
    </div>
</div>





</template>

<style scoped>




h1{
  font-size: 2rem;
  text-align: center;
}

#s{
  margin-top: 0.5rem;
}
.bar{
  margin: 1rem auto;
  border: 2px solid;
  border-radius: 2px;
}

.tier-bar {
  display: flex;
  gap: 10px;
  background-color: gray;
  padding: 10px;

  min-height: 60px;
  align-items: center;
}

.img{
  width: 5%;
  height: 7.5rem;
}



.labels{
  background-color: var(--S);
}
.labela{
  background-color: var(--A);
}
.labelb{
  background-color: var(--B);
}
.labelc{
  background-color: var(--C);
}
.labeld{
  background-color: var(--D);
}
.labele{
  background-color: var(--E);
}
.labelf{
  background-color: var(--F);
}
</style>