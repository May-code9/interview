<template>
  <master-layout :title="'Orders'">
    <div class="home px-5 md:px-7">
      <search-bar></search-bar>
      <order-list></order-list>
    </div>
  </master-layout>
</template>

<script>
// @ is an alias to /src
import MasterLayout from '../components/MasterLayout.vue'
import OrderList from '../components/Orders/OrderList.vue'
import SearchBar from '../components/Orders/SearchBar.vue'

export default {
  name: 'HomePage',
  components: {
    MasterLayout,
    SearchBar,
    OrderList
  }
}
</script>

<style scoped>
.add_order {
  @apply p-4 bg-ezblue-400 text-white rounded-full absolute right-4 bottom-28 cursor-pointer shadow hover:shadow-lg;
}
</style>
