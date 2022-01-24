<template>
  <svg class="inline-block" :class="[width, height]" viewBox="0 0 18 16" fill="none" xmlns="http://www.w3.org/2000/svg">
    <path d="M13 14V16H2V14H13ZM18 7V9H0V7H18ZM16 0V2H5V0H16Z" fill="#1B2022" />
  </svg>
</template>

<script>
export default {
  props: {
    width: {
      default: 'w-5',
      type: String
    },
    height: {
      default: 'h-auto',
      type: String
    }
  }
}
</script>

<style></style>
