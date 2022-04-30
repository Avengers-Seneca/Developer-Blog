<template>
  <DrawerNavigation/>
  <router-view/>
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
</style>
