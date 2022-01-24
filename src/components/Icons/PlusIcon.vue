<template>
  <svg :class="[width, height]" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
    <path
      d="M10.3335 10.3333V0.333252H13.6668V10.3333H23.6668V13.6666H13.6668V23.6666H10.3335V13.6666H0.333496V10.3333H10.3335Z"
      fill="#EEF1EF"
    />
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
      default: 'h-5',
      type: String
    }
  }
}
</script>

<style></style>
