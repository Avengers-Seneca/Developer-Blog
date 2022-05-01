<template>
  <div class="home">
    <ArticlePreviewFeatured />
    <ArticlePreview/>
    <Team/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import ArticlePreviewFeatured from "@/components/ArticlePreviewFeatured.vue";
import Team from "@/components/Team.vue";
import ArticlePreview from "@/components/ArticlePreview.vue";

export default {
  name: "HomeView",
  components: {
    HelloWorld,
    ArticlePreviewFeatured,
    Team,
    ArticlePreview
  },
};
</script>
