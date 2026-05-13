<script setup>
defineProps({
  highlighted: Boolean,
  default: false
})
const emit = defineEmits(['clicked'])
</script>

<template>
  <span @click="emit('clicked')">
    {{ highlighted ? '★' : '☆' }}
  </span>
</template>
