<template>
  <div class="flex justify-between px-5 md:px-7 py-4">
    <div>
      <div class="inline-block text-lg">{{ title }}</div>
    </div>
    <div class="relative">
      <div @click="menu = !menu">
        <three-dots-icon></three-dots-icon>
      </div>
      <div class="rounded-md bg-gray-50 py-2 shadow absolute right-3 top-0" v-if="menu">
        <div class="hover:bg-gray-100 hover:shadow-inner px-6 py-px text-sm" @click="logout">logout</div>
      </div>
    </div>
  </div>
</template>

<script>
import ThreeDotsIcon from './Icons/ThreeDotsIcon.vue'
export default {
  components: { ThreeDotsIcon },
  props: {
    title: String
  },
  data() {
    return {
      menu: false
    }
  },
  methods: {
    //
  }
}
</script>

<style></style>
