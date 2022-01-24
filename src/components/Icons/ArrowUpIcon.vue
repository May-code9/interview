<template>
  <svg
    xmlns="http://www.w3.org/2000/svg"
    class="fill-current inline"
    :class="[width, height]"
    viewBox="0 0 11.749 6.285"
  >
    <path
      id="Icon_metro-chevron-thin-down"
      data-name="Icon metro-chevron-thin-down"
      d="M15.671,10.792a.476.476,0,0,1,.669,0,.464.464,0,0,1,0,.662l-5.4,5.349a.476.476,0,0,1-.669,0l-5.4-5.349a.465.465,0,0,1,0-.662.476.476,0,0,1,.669,0L10.6,15.67Z"
      transform="translate(16.479 16.94) rotate(180)"
      fill="#9698b6"
    />
  </svg>
</template>

<script>
export default {
  props: {
    width: {
      type: String,
      default: 'w-3'
    },
    height: {
      type: String,
      default: 'h-1'
    }
  }
}
</script>
