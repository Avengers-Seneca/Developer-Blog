<template>
  
    <DrawerNavigation />
    <div data-theme="dark">
    <main class="container yx-t max-width-adaptive-md yx-sg">
      <router-view />
    </main>
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import DrawerNavigation from "@/components/DrawerNavigation.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "App",
  components: {
    DrawerNavigation,
    Footer,
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
