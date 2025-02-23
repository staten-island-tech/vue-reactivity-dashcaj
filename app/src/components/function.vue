<template>
    



 

</template>

<script>    
import { listofimages, cycle, noimg} from './image.vue';
import { ref } from 'vue';

export const tierS = ref([]);
export const tierA = ref([]);
export const tierB = ref([]);
export const tierC = ref([]);
export const tierD = ref([]);
export const tierE = ref([]);
export const tierF = ref([]);

export function addtotier(tier) {
  if (noimg.value) return;

  if (listofimages.value.length > 0) {
    const newItem = { id: tier.value.length + 1, img: listofimages.value[0] };
    tier.value.push(newItem);
    cycle(); // Cycle to the next image
  }
}




</script>