<template>


</template>

<script>    
import { ref } from 'vue';
export const listofimages = ref([
    '@/imgs/71PMJAJqUIL._AC_UF1000,1000_QL80_.jpg',
    '@/imgs/81+jwWMXYrL._AC_UF350,350_QL80_.jpg',
    '@/imgs/11619607_hi.jpg',
    '@/imgs/download (1).jpg',
    '@/imgs/download (2).jpg',
    '@/imgs/download (3).jpg',
    '@/imgs/download (4).jpg',
    '@/imgs/download (5).jpg',
    '@/imgs/download (6).jpg',
    '@/imgs/download (7).jpg',
    '@/imgs/download.jpg',
    '@/imgs/download.png',
    '@/imgs/mp-4510-1000px.webp',
    '@/imgs/New-York-Nights__PRODUCT_01--IMG_ZOOM--NEWYORKNIGHTS-1875665158.png',
    '@/imgs/tf_sku_T01K01_2000x2000_1.webp'
])

export const noimg = ref(false);

// Function to cycle images
export function cycle() {
  if (listofimages.value.length === 0) {
    noimg.value = true;
    return;
  }
  const img1 = listofimages.value.shift();
  listofimages.value.push(img1);
}
</script>