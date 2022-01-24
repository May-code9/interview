<template>
  <svg
    xmlns="http://www.w3.org/2000/svg"
    class="fill-current inline"
    :class="[width, height, color]"
    viewBox="0 0 24.001 24"
  >
    <path
      id="close"
      d="M3.513,20.485a12,12,0,1,1,16.972,0A12,12,0,0,1,3.513,20.485ZM18.364,5.635a9,9,0,1,0,0,12.728A9,9,0,0,0,18.364,5.635ZM8.817,17.3,6.7,15.181,9.878,12,6.7,8.818,8.817,6.7,12,9.878,15.181,6.7,17.3,8.818,14.12,12,17.3,15.181,15.181,17.3,12,14.121,8.817,17.3Z"
      transform="translate(0.002 0)"
      fill="#848b96"
    />
  </svg>
</template>

<script>
export default {
  props: {
    width: String,
    height: String,
    color: String
  }
}
</script>

<style></style>
