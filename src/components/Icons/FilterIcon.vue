<template>
  <svg :class="[width, height]" viewBox="0 0 16 19" fill="none" xmlns="http://www.w3.org/2000/svg">
    <path d="M10 11V17L6 19V11L0 2V0H16V2L10 11ZM2.404 2L8 10.394L13.596 2H2.404Z" fill="#0994C9" />
  </svg>
</template>

<script>
export default {
  props: {
    width: {
      default: 'w-4',
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
