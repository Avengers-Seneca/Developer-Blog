<template>
  <div class="home">
    <ArticlePreviewFeatured :featuredArticle="featuredArticle" />
    <div :key="article.id" v-for="article in articles">
      <ArticlePreview :article="article" />
    </div>
    <Team />
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
    ArticlePreview,
  },
  data() {
    return {
      articles: [],
      featuredArticle: new Object(),
    };
  },
  methods: {
    // async fetchArticles() {
    //   const res = await fetch('api/articles')

    //   const data = await res.json()

    //   return data
    // },
    fetchArticles() {
      let data = [
        {
          id: 1,
          title: "A sample Blog 1",
          content:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. At iusto sit quasi aliquam quod laboriosam. Nobis, modi repellendus.",
          author: "Alice Han",
          datePublished: "May 1, 2022",
          tag: "Programming",
          authorImg: "img/article-preview-img-author-1.svg",
          articleImg: "img/article-preview-img-2.jpg",
          isFeatured: true,
        },
        {
          id: 2,
          title: "A sample Blog 2",
          content:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. At iusto sit quasi aliquam quod laboriosam. Nobis, modi repellendus.",
          author: "Alice Han",
          datePublished: "May 1, 2022",
          tag: "Programming",
          authorImg: "img/article-preview-img-author-1.svg",
          articleImg: "img/article-preview-img-2.jpg",
          isFeatured: true,
        },
        {
          id: 3,
          title: "A sample Blog 3",
          content:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. At iusto sit quasi aliquam quod laboriosam. Nobis, modi repellendus.",
          author: "John Doe",
          datePublished: "May 1, 2022",
          tag: "Programming",
          authorImg: "img/article-preview-img-author-1.svg",
          articleImg: "img/article-preview-img-2.jpg",
          isFeatured: true,
        },
        {
          id: 4,
          title: "A sample Blog 4",
          content:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. At iusto sit quasi aliquam quod laboriosam. Nobis, modi repellendus.",
          author: "Jane Doe",
          datePublished: "May 1, 2022",
          tag: "Programming",
          authorImg: "img/article-preview-img-author-1.svg",
          articleImg: "img/article-preview-img-2.jpg",
          isFeatured: false,
        },
      ];
      return data;
    },
  },
  created() {
    this.articles = this.fetchArticles().filter(article => article.isFeatured).slice(1);
    this.featuredArticle = this.fetchArticles().find((a) => a.isFeatured);
  },
};
</script>
