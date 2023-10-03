<script setup>
import { onMounted } from 'vue'
import { initFlowbite } from 'flowbite'

// initialize components based on data attribute selectors
onMounted(() => {
    initFlowbite();
})
</script>
<template>
    <div>
        
<figure class="relative max-w-sm transition-all duration-300 cursor-pointer filter grayscale hover:grayscale-0">
  <a href="#">
    <img class="rounded-lg" src="https://images5.alphacoders.com/681/681402.jpg" alt="image description">
  </a>
  <figcaption class="absolute px-4 text-lg text-white bottom-6">
      <p>WELCOME</p>
  </figcaption>
</figure>

    </div>
</template>