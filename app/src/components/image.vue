<template>


</template>

<script>    
import { ref } from 'vue';
export const originalimages = [
    'https://creedboutique.com/cdn/shop/files/aventus-100ml-bottle_3413e5f4-3eee-40b3-8451-2546a370ec5b.jpg?v=1734710265&width=750',
    'https://m.media-amazon.com/images/I/81+jwWMXYrL._AC_UF350,350_QL80_.jpg',
    'https://cdn.media.amplience.net/s/hottopic/11619607_hi',
    'https://m.media-amazon.com/images/I/71Vyjtw637L.jpg',
    'https://www.sephora.com/productimages/product/p449122-av-1-zoom.jpg',
    'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQpqrbsRN494h-XsthBSm5tGSQU2cxrZvpVZw&s',
    'https://dimg.dillards.com/is/image/DillardsZoom/mainProduct/viktor--rolf-spicebomb-extreme-eau-de-parfum/05157632_zi.jpg',
    'https://m.media-amazon.com/images/I/412TXqfY5jL.jpg',
    'https://m.media-amazon.com/images/I/61YIgukdRgL.jpg',
    'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSpvXH5DclPCwH2SJoznEP8EWRuM-O8wOktZg&s',
    'https://m.media-amazon.com/images/I/41FB87Tvl4L._AC_.jpg',
    'https://m.media-amazon.com/images/I/61WTqMHzC3L.jpg',
    'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQne8BOMqh-T1QKq1jDNmFIeqq8AbsviH_54g&s',
    'https://media.maxaroma.com/9cd29e92-4b8f-436f-ad1f-8e368b30dc1d/https://www.maxaroma.com/productimages/large/UP888874007741.jpg?ver=1701625686',
    'https://www.sephora.com/productimages/sku/s1449297-main-zoom.jpg'
]

export const listofimages = ref([...originalimages]);








/* export const noimg = ref(false);


export function cycle() {
  if (listofimages.value.length === 0) {
    noimg.value = true;
    return;
  }
  const img1 = listofimages.value.shift();
  listofimages.value.push(img1);
} */
</script>