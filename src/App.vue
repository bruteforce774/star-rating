<script setup>
import Star from './components/Star.vue'

function handleClick() {
  console.log('Star was clicked!')
}
</script>

<template>
  <Star @clicked="handleClick" />
</template>
