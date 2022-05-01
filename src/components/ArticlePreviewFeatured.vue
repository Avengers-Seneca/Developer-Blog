<template>
  <div class="margin-bottom-lg text-center">
    <h1>Featured Blog</h1>
  </div>
  <article class="story story--featured">
    <a class="story__img radius-md" href="#0">
      <figure class="aspect-ratio-4:3">
        <img src="img/article-preview-img-2.jpg" alt="Image description" />
      </figure>
    </a>

    <div class="story__content">
      <div class="margin-bottom-xs">
        <a class="story__category" href="#0">
          <svg
            class="icon margin-right-xxxs"
            aria-hidden="true"
            viewBox="0 0 16 16"
          >
            <g
              stroke-width="1"
              stroke="currentColor"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
            >
              <circle cx="8" cy="7" r="1.5"></circle>
              <path d="M12.121,14.263a7.5,7.5,0,1,0-8.242,0"></path>
              <path d="M12.377,11.32a5.5,5.5,0,1,0-8.754,0"></path>
              <path
                d="M6.605,10.5H9.4a1,1,0,0,1,1,1.1L10,15.5H6l-.39-3.9A1,1,0,0,1,6.605,10.5Z"
              ></path>
            </g>
          </svg>
          <i>Podcast</i>
        </a>
      </div>

      <div class="text-component">
        <h2 class="story__title">
          <a href="#0"
            >Lorem ipsum dolor sit, amet consectetur adipisicing elit.</a
          >
        </h2>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. At iusto sit
          quasi aliquam quod laboriosam. Nobis, modi repellendus.
        </p>
      </div>

      <div class="story__author margin-top-sm">
        <a class="block" href="#0">
          <img
            src="img/article-preview-img-author-1.svg"
            alt="Author picture"
          />
        </a>

        <div class="line-height-xs">
          <address class="story__author-name">
            <a href="#0" rel="author">Olivia Gribben</a>
          </address>
          <p class="story__meta"><time>May 16</time> &mdash; 5 min read</p>
        </div>
      </div>
    </div>
  </article>
</template>

<script>
export default {
  name: "ArticlePreviewFeatured",
};
</script>

<style lang="scss" scoped>
@use "../../node_modules/codyhouse-framework/main/assets/css/base/breakpoints"
  as *;
@use "../../node_modules/codyhouse-framework/main/assets/css/base/mixins" as *;

@use "../assets/css/custom-style/article-preview--featured" as *;
</style>