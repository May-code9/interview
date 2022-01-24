<template>
  <master-layout :title="'Orders'">
    <div class="home px-5 md:px-7">
      
    </div>
  </master-layout>
</template>

<script>
// @ is an alias to /src
import MasterLayout from '../components/MasterLayout.vue'

export default {
  name: 'HomePage',
  components: {
    MasterLayout
  }
}
</script>

<style scoped>
.add_order {
  @apply p-4 bg-ezblue-400 text-white rounded-full absolute right-4 bottom-28 cursor-pointer shadow hover:shadow-lg;
}
</style>
