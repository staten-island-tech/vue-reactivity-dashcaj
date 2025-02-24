<template>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Atkinson+Hyperlegible+Next:ital,wght@0,200..800;1,200..800&family=Reddit+Sans+Condensed:wght@200..900&family=Roboto:ital,wght@0,100..900;1,100..900&display=swap" rel="stylesheet">



  <thetitle/>
  <div class="ui">
    <img class="images" v-if="listofimages.length" :src="listofimages[0]" alt="">
    <p class="flag" v-if="!listofimages.length">no more images</p>
      <div class="buttons">
        <button class="btn" id="S" @click="cycleS">s</button>
        <button class="btn" id="A" @click="cycleA">a</button>
        <button class="btn" id="B" @click="cycleB">b</button>
        <button class="btn" id="C" @click="cycleC">c</button>
        <button class="btn" id="D" @click="cycleD">d</button>
        <button class="btn" id="E" @click="cycleE">e</button>
        <button class="btn" id="F" @click="cycleF">f</button>
      </div>
      
  <button class="reset"@click="resetbtn">Reset?</button>

      
  </div>

  <TierChart/>
</template>

<script setup>
import TierChart from '@/components/tiersection.vue'
import { listofimages, originalimages } from '@/components/image.vue';
import thetitle from '@/components/thetitle.vue';
import { tiers } from '@/components/ALLTIERS.vue'
import { cycleS, cycleA, cycleB, cycleC, cycleD, cycleE, cycleF } from '@/components/buttontiers.vue';

const resetbtn = () => {
  listofimages.value = [...originalimages]; 

  Object.keys(tiers).forEach((tier) => {
    tiers[tier].length = 0;
  });
};
</script>




<style scoped>
.titles{
    text-align: center;
    font-size: 7rem;
    margin: 3rem auto;
}

.ui{
  text-align: center;
}

.images{
  width: 17%;
  height: 35rem;
  margin: 3rem;
  margin-bottom: 1rem;
  border: 3px solid;
  background-color: var(--2color);
  padding: 1rem;
}



.btn{
  font-size: 2rem;
  padding-left: 15rem;
  padding-right: 15rem;
  margin: 0.25rem auto;
  display: flex;
  justify-content: space-between;
  border-radius: 2px;
}

.btn:hover{
  background-color: rgb(40, 40, 40);
  color: antiquewhite;
  transition: transform 1s ease;
}

.flag{
  font-size: 12rem;
}

.reset{
  font-size: 2rem;
  padding-left: 15rem;
  padding-right: 15rem;
  text-align: center;
  margin-top: 5rem;
  background-color: var(--2color);
}













#S{
  background-color: var(--S);
}

#A{
  background-color: var(--A);
}
#B{
  background-color: var(--B);
}
#C{
  background-color: var(--C);
}
#D{
  background-color: var(--D);
}
#E{
  background-color: var(--E);
}
#F{
  background-color: var(--F);
}



</style>
