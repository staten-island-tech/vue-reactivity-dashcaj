<template>

</template>

<script>
import { tierS, tierA, tierB, tierC, tierD, tierE, tierF } from "@/components/ALLTIERS.vue"
import { listofimages } from "./image.vue";



export function cycleS() {
    const firstimage = listofimages.value.shift()
  tierS.value.push(firstimage)
}

export function cycleA() {
    const firstimage = listofimages.value.shift()
  tierA.value.push(firstimage)
}

export function cycleB() {
    const firstimage = listofimages.value.shift()
  tierB.value.push(firstimage)
}

export function cycleC() {
    const firstimage = listofimages.value.shift()
  tierC.value.push(firstimage)
}

export function cycleD() {
    const firstimage = listofimages.value.shift()
  tierD.value.push(firstimage)
}

export function cycleE() {
    const firstimage = listofimages.value.shift()
  tierE.value.push(firstimage)
}

export function cycleF() {
    const firstimage = listofimages.value.shift()
  tierF.value.push(firstimage)
}


</script>

