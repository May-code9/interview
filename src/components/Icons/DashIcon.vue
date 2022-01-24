<template>
  <svg :class="[width, height]" viewBox="0 0 36 4" fill="none" xmlns="http://www.w3.org/2000/svg">
    <rect width="36" height="4" rx="2" :fill="color" />
  </svg>
</template>

<script>
export default {
  props: {
    width: {
      default: 'w-8',
      type: String
    },
    height: {
      default: 'h-auto',
      type: String
    },
    color: {
      default: '#D4D8D5',
      type: String
    }
  }
}
</script>

<style></style>
