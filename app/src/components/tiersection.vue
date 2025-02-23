

<script>
import { defineProps } from 'vue';
import { addtotier } from './function.vue';

const props = defineProps({
  tier: {
    type: Array,
    required: true,
  },
  appendtotier: Function,
  noimages: Boolean,
  tiername: String
});

</script>

<template>
    <div class="tier-container">
        <h3 class="tier-title">{{ tierName }} Tier</h3>
        <div class="tier-bar">
        <img v-for="item in props.tier" :key="item.id" :src="item.img" alt="Added Image" class="tier-image" />
    </div>

    <button @click="props.addToTier(props.tier)" :disabled="props.noMoreImages">
      Add Image to {{ tierName }} Tier
    </button>
  </div>

</template>