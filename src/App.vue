<template>
  <div class="bg-gray-100">
    <div
      class="max-w-screen-sm mx-auto h-screen bg-ezwhite-100 sm:border border-ezblack-200 relative text-left"
    >
      <router-view v-slot="{ Component }">
        <transition name="view">
          <component :is="Component" />
        </transition>
      </router-view>
    </div>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
