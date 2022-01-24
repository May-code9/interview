<template>
  <div class="flex flex-col h-screen justify-between">
    <div class="overflow-y-auto">
      <top-layer :title="$attrs.title"></top-layer>
      <slot></slot>
    </div>
    <bottom-layer :title="$attrs.title"></bottom-layer>
  </div>
</template>

<script>
import BottomLayer from './BottomLayer.vue'
import TopLayer from './TopLayer.vue'

export default { components: { TopLayer, BottomLayer } }
</script>

<style></style>
