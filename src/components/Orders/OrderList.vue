<template>
  <div>
    <div class="bg-ezblue-400 rounded-lg text-white px-4 py-3">
      <div class="flex justify-between">
        <div>Total Orders</div>
        <div class="font-extrabold">62</div>
      </div>
    </div>
    <div class="my-4 py-3 px-4 rounded-lg border border-ezblack-300 shadow-md" v-for="(order, index) in orders" :key="index">
      <div class="flex justify-between items-center">
        <div class="font-medium">{{ order.id }}</div>
        <div
          class="text-xs"
          :class="{
            'text-ezgreen-200': order.status == 'delivered',
            'text-ezyellow-200': order.status == 'in progress'
          }"
        >
          {{ order.status }}
        </div>
      </div>
      <div class="text-xs">{{ order.item }}</div>
      <div class="flex items-center pt-3">
        <div class="text-xs mr-2 text-ezblack-300">
          <div class="pb-2">{{ order.start_date }}</div>
          <div>{{ order.end_date }}</div>
        </div>
        <div>
          <divider-icon :width="'w-2'" :height="'h-6'"></divider-icon>
        </div>
        <div class="text-xs ml-2 text-ezblack-400">
          <div class="pb-2">{{ order.pick }}</div>
          <div>{{ order.drop }}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import DividerIcon from '../Icons/DividerIcon.vue'
export default {
  components: { DividerIcon },
  data() {
    return {
      orders: [
        {
          id: '2435743',
          status: 'delivered',
          item: 'A hand bag',
          start_date: 'Mar 29',
          end_date: 'Mar 30',
          pick: '234, adekunle gold street, lagos',
          drop: '567, marina estate, lagos'
        },
        {
          id: '4356354',
          status: 'pending',
          item: 'Document',
          start_date: 'Mar 30',
          end_date: 'Mar 30',
          pick: '234, adekunle gold street, lagos',
          drop: '567, marina estate, lagos'
        },
        {
          id: '988656',
          status: 'in progress',
          item: 'Food',
          start_date: 'April 1',
          end_date: 'April 2',
          pick: '234, adekunle gold street, lagos',
          drop: '567, marina estate, lagos'
        }
      ]
    }
  }
}
</script>

<style></style>
