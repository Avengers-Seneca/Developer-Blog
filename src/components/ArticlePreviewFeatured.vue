<template>
<article class="story story--featured">
    <a class="story__img radius-md" href="#0">
      <figure class="aspect-ratio-4:3">
        <img
          src="img/article-preview-img-2.jpg"
          alt="Image description"
        />
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

<style scoped>
/* -------------------------------- 

File#: _1_article-preview
Title: Article Preview
Descr: Blog post excerpt, containing a link to the article page
Usage: codyhouse.co/license

-------------------------------- */
.story__img {
  display: block;
  transition: opacity 0.2s;
  overflow: hidden;
  margin-bottom: var(--space-xs);
}
.story__img:hover {
  opacity: 0.85;
}
.story__img img {
  display: block;
  width: 100%;
}

.story__category {
  display: inline-flex;
  align-items: center;
  color: var(--color-contrast-higher);
  line-height: 1;
  text-decoration: none;
  font-size: var(--text-sm);
  background-color: hsla(
    var(--color-primary-h),
    var(--color-primary-s),
    var(--color-primary-l),
    0.2
  );
  padding: var(--space-xxs);
  border-radius: var(--radius-md);
  transition: background-color 0.2s;
}
.story__category:hover {
  text-decoration: underline;
  background-color: hsla(
    var(--color-primary-h),
    var(--color-primary-s),
    var(--color-primary-l),
    0.3
  );
}

.story__title a {
  color: var(--color-contrast-higher);
  text-decoration: none;
}
.story__title a:hover {
  text-decoration: underline;
}

.story__author {
  --author-img-size: 50px;
  display: grid;
  grid-template-columns: var(--author-img-size) 1fr;
  align-items: center;
  gap: var(--space-xs);
}
.story__author img {
  display: block;
  width: var(--author-img-size);
  height: var(--author-img-size);
  -o-object-fit: cover;
  object-fit: cover;
  border-radius: 50%;
}

.story__author-name {
  margin-bottom: var(--space-xxxxs);
}
.story__author-name a {
  text-decoration: none;
  color: var(--color-contrast-higher);
}
.story__author-name a:hover {
  text-decoration: underline;
}

.story__meta {
  font-size: var(--text-sm);
  color: var(--color-contrast-medium);
}

@media (min-width: 64rem) {
  .story--featured {
    display: grid;
    grid-template-columns: 3fr 2fr;
    grid-gap: var(--space-md);
    align-items: center;
  }
  .story--featured .story__img {
    margin: 0;
  }
  .story--featured .story__title {
    font-size: var(--text-xxl);
  }
}
</style>