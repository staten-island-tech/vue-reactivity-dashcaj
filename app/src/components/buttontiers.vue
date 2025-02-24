<template>

</template>

<script>
import { tiers } from "@/components/ALLTIERS.vue"
import { listofimages } from "./image.vue";



export function cycleS() {
  const firstimage = listofimages.value.shift()
  tiers.tierS.push(firstimage)
}

export function cycleA() {
  const firstimage = listofimages.value.shift()
  tiers.tierA.push(firstimage)
}

export function cycleB() {
  const firstimage = listofimages.value.shift()
  tiers.tierB.push(firstimage)
}

export function cycleC() {
  const firstimage = listofimages.value.shift()
  tiers.tierC.push(firstimage)
}

export function cycleD() {
  const firstimage = listofimages.value.shift()
  tiers.tierD.push(firstimage)
}

export function cycleE() {
  const firstimage = listofimages.value.shift()
  tiers.tierE.push(firstimage)
}

export function cycleF() {
  const firstimage = listofimages.value.shift()
  tiers.tierF.push(firstimage)
}


</script>

