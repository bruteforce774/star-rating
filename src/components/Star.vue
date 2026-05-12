<script setup>
defineProps({
  highlighted: Boolean
})
const emit = defineEmits(['clicked'])
</script>

<template>
  <span @click="emit('clicked')">
    {{ highlighted ? '★' : '☆' }}
  </span>
</template>
