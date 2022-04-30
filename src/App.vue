<template>
  <DrawerNavigation />
  <main class="container yx-t max-width-adaptive-lg yx-sg">
    <router-view />
  </main>
</template>

<script>
// @ is an alias to /src
import DrawerNavigation from "@/components/DrawerNavigation.vue";

export default {
  name: "App",
  components: {
    DrawerNavigation,
  },
};
</script>

<style>
.container {
  width: calc(100% - 2 * 1.25rem);
  margin-left: auto;
  margin-right: auto;
  padding: 1.25rem 0;
}
</style>
