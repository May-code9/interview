<template>
  <svg
    class="fill-current inline-block"
    :class="[width, height]"
    viewBox="0 0 8 32"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      d="M4 8C6.20914 8 8 6.20914 8 4C8 1.79086 6.20914 0 4 0C1.79086 0 0 1.79086 0 4C0 6.20914 1.79086 8 4 8Z"
      fill="#49565B"
    />
    <path d="M3.8 24V8" stroke="#49565B" stroke-width="0.4" />
    <path
      d="M4 32C6.20914 32 8 30.2091 8 28C8 25.7909 6.20914 24 4 24C1.79086 24 0 25.7909 0 28C0 30.2091 1.79086 32 4 32Z"
      fill="#49565B"
    />
  </svg>
</template>

<script>
export default {
  props: {
    width: {
      default: 'w-1',
      type: String
    },
    height: {
      default: 'h-4',
      type: String
    }
  }
}
</script>

<style></style>
