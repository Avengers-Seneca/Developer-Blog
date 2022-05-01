<template>

  <section class="team padding-y-xl">
    <div class="container max-width-adaptive-lg">
      <div class="margin-bottom-lg text-center ">
        <h1>Meet Our Team.</h1>
      </div>

      <div class="grid gap-sm">
        <div class="card-v2 radius-md col-3@md">
          <figure>
            <img
              src="img/team-img-1.jpg"
              alt="Image description"
            />
            <figcaption
              class="
                card-v2__caption
                padding-x-sm padding-top-md padding-bottom-sm
                text-center
              "
            >
              <div class="text-md text-base@md">Alice Han</div>
              <div class="margin-top-xxxs text-sm opacity-70%">Back-End Developer</div>
            </figcaption>
          </figure>
        </div>

        <div class="card-v2 radius-md col-3@md">
          <figure>
            <img
              src="img/team-img-2.jpg"
              alt="Image description"
            />
            <figcaption
              class="
                card-v2__caption
                padding-x-sm padding-top-md padding-bottom-sm
                text-center
              "
            >
              <div class="text-md text-base@md">Ravni Arador</div>
              <div class="margin-top-xxxs text-sm opacity-70%">Front-End Developer</div>
            </figcaption>
          </figure>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
    name: "Team"
}
</script>

<style lang="scss" scoped>
@use "../../node_modules/codyhouse-framework/main/assets/css/base/breakpoints"
  as *;
@use "../../node_modules/codyhouse-framework/main/assets/css/base/mixins" as *;

@use "../assets/css/custom-style/team" as *;
</style>