<script setup>
import { ref } from 'vue'
import Star from './Star.vue'

const rating = ref(0)

function setRating(value) {
  rating.value = value
}
</script>

<template>
  <Star
    v-for="n in 5"
    :key="n"
    :highlighted="n <= rating"
    @clicked="setRating(n)"
  />
</template>
