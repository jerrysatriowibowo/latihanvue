<script setup>
import { Rating } from 'flowbite-vue'
</script>
<template>
    <Rating :rating="1" :scale="1" review-text="2456 reviews">
      <template #besideText>
        <p class="ml-2 text-sm font-bold text-gray-900 dark:text-white">4.75</p>
      </template>
    </Rating>
</template>