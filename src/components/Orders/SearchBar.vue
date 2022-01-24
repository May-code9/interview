<template>
  <div class="flex items-center justify-between mb-3">
    <div class="w-full relative">
      <input
        class="rounded-lg pl-4 pr-11 py-3 border border-ezblack-300 bg-ezwhite-100 w-full focus:outline-none focus:shadow-inner"
        placeholder="Looking for..."
      />
      <div class="absolute top-4 right-3 -mt-px">
        <search-icon></search-icon>
      </div>
    </div>
    <div class="rounded-lg border border-ezblue-300 py-4 px-4 ml-2 cursor-pointer shadow focus:shadow-lg">
      <filter-icon></filter-icon>
    </div>
  </div>
</template>

<script>
import FilterIcon from '../Icons/FilterIcon.vue'
import SearchIcon from '../Icons/SearchIcon.vue'
export default {
  components: { SearchIcon, FilterIcon }
}
</script>

<style></style>
