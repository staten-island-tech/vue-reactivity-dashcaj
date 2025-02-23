<template>
  <div class="parent-container">
    <!-- Title component -->
    <thetitle />

    <!-- Tier components: Each gets the respective tier array, the addToTier function, and the noMoreImages flag -->
    <tiers :tier="tierS" :addToTier="addtotier" :noMoreImages="noimg" tierName="S" />
    <tiers :tier="tierA" :addToTier="addtotier" :noMoreImages="noimg" tierName="A" />
    <tiers :tier="tierB" :addToTier="addtotier" :noMoreImages="noimg" tierName="B" />
    <tiers :tier="tierC" :addToTier="addtotier" :noMoreImages="noimg" tierName="C" />
    <tiers :tier="tierD" :addToTier="addtotier" :noMoreImages="noimg" tierName="D" />
    <tiers :tier="tierE" :addToTier="addtotier" :noMoreImages="noimg" tierName="E" />
    <tiers :tier="tierF" :addToTier="addtotier" :noMoreImages="noimg" tierName="F" />
  </div>


</template>

<script setup>
import { tierS, tierA, tierB, tierC, tierD, tierE, tierF, addtotier } from '@/components/function.vue';
import { noimg } from '@/components/image.vue';
import tiers from '@/components/tiersection.vue';
import thetitle from '@/components/thetitle.vue';
</script>

<style scoped>
p{
  font-size: 30px;
}

button{
  font-size: 30px;
}
</style>