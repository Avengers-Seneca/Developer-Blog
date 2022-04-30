<template>
  <div class="home">
    <ArticlePreviewFeatured />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import ArticlePreviewFeatured from "@/components/ArticlePreviewFeatured.vue";

export default {
  name: "HomeView",
  components: {
    HelloWorld,
    ArticlePreviewFeatured,
  },
};
</script>
