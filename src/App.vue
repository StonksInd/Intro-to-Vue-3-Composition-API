<script setup>
import { ref } from 'vue'
import socksGreenImage from './assets/images/socks_green.jpeg'
import socksBlueImage from './assets/images/socks_blue.jpeg'
const product = ref('Socks')
const image = ref(socksBlueImage)
const url = ref( 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQhNhtqtnswc6iC8kfqbAp70bKxbkRTogHLXJW56o0njSQBQDPsY4bkHEOQCivVd4-lamBr2rg9F9CnyYRlFpzaIpS69gkDGkGOvYA_b61w')
</script>

<template>
  <div class="product-display">
    <div class="product-container">
      <div class="product-image">
        <img :src="image" alt="">
        <img :src="url" alt="">
      </div>
      <div class="product-info">
        <h1>{{ product }}</h1>
      </div>
    </div>
  </div>
</template>