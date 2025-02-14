<template>


</template>

<script>    
import { ref } from 'vue';
export const listofimages = ref([1,2,3,4,5,6,7,8,9,1])

export function cycle() {
    listofimages.value.shift()
}
</script>