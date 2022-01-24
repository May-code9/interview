<template>
  <div class="border-2 border-ezblue-400 rounded-full inline-block p-1">
    <div class="rounded-full p-1" :class="{ 'bg-ezblue-400': checked, 'bg-ezblack-100': !checked }"></div>
  </div>
</template>

<script>
export default {
  props: {
    checked: {
      default: false,
      type: Boolean
    }
  }
}
</script>

<style scoped>
.pad__1 {
  padding: 0.2rem;
}
</style>
