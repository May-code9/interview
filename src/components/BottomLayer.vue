<template>
  <div class="border-t bg-ezwhite-100 upper_shadow">
    <div class="flex justify-between items-center px-5 md:px-7">
      <router-link
        :to="{ name: 'Home' }"
        class="border-t py-4 hover:border-ezblue-400"
        :class="{ 'border-ezblue-400': title == 'Orders', 'border-transparent': title != 'Orders' }"
      >
        <orders-icon v-if="title == 'Orders'" :fill="'#0994C9'"></orders-icon>
        <orders-icon v-else></orders-icon>
      </router-link>
      <div
        class="py-4 border-t hover:border-ezblue-400"
        :class="{ 'border-ezblue-400': title == 'Wallet', 'border-transparent': title != 'Wallet' }"
      >
        <wallet-icon v-if="title == 'Wallet'" :fill="'#0994C9'"></wallet-icon>
        <wallet-icon v-else></wallet-icon>
      </div>
      <div
        class="py-4 border-t hover:border-ezblue-400"
        :class="{ 'border-ezblue-400': title == 'Clients', 'border-transparent': title != 'Clients' }"
      >
        <client-icon v-if="title == 'Clients'" :fill="'#0994C9'"></client-icon>
        <client-icon v-else></client-icon>
      </div>
      <div class="py-4 border-t border-transparent hover:border-ezblue-400">
        <profile-icon></profile-icon>
      </div>
    </div>
  </div>
</template>

<script>
import ClientIcon from './Icons/ClientIcon.vue'
import OrdersIcon from './Icons/OrdersIcon.vue'
import ProfileIcon from './Icons/ProfileIcon.vue'
import WalletIcon from './Icons/WalletIcon.vue'
export default {
  components: { OrdersIcon, WalletIcon, ClientIcon, ProfileIcon },
  props: {
    title: String
  }
}
</script>

<style scoped>
.upper_shadow {
  box-shadow: -1px -3px 7px 2px rgba(156, 155, 155, 0.2);
  -webkit-box-shadow: -1px -3px 7px 2px rgba(156, 155, 155, 0.2);
  -moz-box-shadow: -1px -3px 7px 2px rgba(156, 155, 155, 0.2);
}
</style>
