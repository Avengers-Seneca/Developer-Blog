<template>
  <header class="dr-nav-header">
    <div class="container position-relative height-100% flex items-center">
      <router-link class="dr-nav-header__logo" to="/">
        <svg viewBox="0 0 64 64">
          <title>Go to homepage</title>
          <path
            fill="currentColor"
            d="M32 1a31 31 0 1031 31A31 31 0 0032 1zm15.189 17.262a5.693 5.693 0 00-2.169 1.686 11.279 11.279 0 00-1.891 3.552l-9.281 25.119q-.495-.043-1.547-.043-1.011 0-1.483.043L19.582 21.076a5.357 5.357 0 00-1.3-2.116 2.47 2.47 0 00-1.471-.7v-.881q2.642.129 6.7.129 4.49 0 6.681-.129v.881a6.764 6.764 0 00-2.374.4 1.236 1.236 0 00-.718 1.24 6.34 6.34 0 00.537 2.062l7.756 19.7 5.416-14.592a17.5 17.5 0 001.224-5.37 3.216 3.216 0 00-.934-2.567 4.374 4.374 0 00-2.761-.87v-.881q2.964.129 5.5.129 2.019 0 3.351-.129z"
          />
        </svg>
      </router-link>

      <button class="btn btn--basic" aria-controls="modal-login">Login</button>
      <button class="btn btn--basic" aria-controls="modal-register">
        Register
      </button>
    </div>
  </header>

  <div class="drawer js-drawer" id="dr-nav-id">
    <div
      class="drawer__content bg-light inner-glow shadow-md"
      role="alertdialog"
      aria-labelledby="dr-nav-title"
    >
      <div class="drawer__body flex flex-column js-drawer__body">
        <header class="dr-nav-drawer-header padding-x-md">
          <h4 id="dr-nav-title">Menu</h4>
        </header>

        <nav class="dr-nav padding-md" aria-label="Main">
          <ul>
            <li>
              <router-link class="dr-nav__link" to="/">
                <span>Home</span>
                <span></span>
              </router-link>
            </li>

            <li>
              <a class="dr-nav__link" href="#0">
                <span>Create Post</span>
                <span></span>
              </a>
            </li>

            <li>
              <a class="dr-nav__link" href="#0">
                <span>Tags</span>
                <span></span>
              </a>
            </li>

            <li>
              <a class="dr-nav__link" href="#0">
                <span>About</span>
                <span></span>
              </a>
            </li>
          </ul>
        </nav>

        <footer class="padding-md margin-top-auto">
          <div class="search-input search-input--icon-right">
            <input
              class="search-input__input form-control"
              type="search"
              placeholder="Search..."
              aria-label="Search"
            />
            <button class="search-input__btn">
              <svg class="icon" viewBox="0 0 20 20">
                <title>Submit</title>
                <g
                  fill="none"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                >
                  <circle cx="8" cy="8" r="6" />
                  <line x1="12.242" y1="12.242" x2="18" y2="18" />
                </g>
              </svg>
            </button>
          </div>
        </footer>
      </div>
    </div>
  </div>

  <div class="dr-nav-control-wrapper">
    <div class="container height-100% flex items-center">
      <button
        class="
          reset
          margin-left-auto
          dr-nav-control
          anim-menu-btn
          js-anim-menu-btn js-dr-nav-control js-tab-focus
        "
        aria-label="Toggle navigation"
        aria-controls="dr-nav-id"
      >
        <svg class="dr-nav-control__bg" aria-hidden="true" viewBox="0 0 48 48">
          <circle cx="24" cy="24" r="22" stroke-miterlimit="10" />
        </svg>
        <i
          class="anim-menu-btn__icon anim-menu-btn__icon--arrow-right"
          aria-hidden="true"
        ></i>
      </button>
    </div>
  </div>

  <div
    data-theme="dark"
    class="
      modal modal--animate-scale
      bg bg-opacity-99%
      flex flex-center
      padding-md
      js-modal
    "
    id="modal-login"
  >
    <div
      class="
        modal__content
        max-width-xs max-height-100%
        overflow-auto
        padding-md
        text-center
      "
      role="alertdialog"
      aria-labelledby="modal-select-title"
      aria-describedby=""
    >
      <p
        class="color-contrast-medium margin-bottom-xs"
        id="modal-select-title"
      ></p>

      <ul
        class="
          full-screen-select
          flex flex-column
          gap-xxs
          js-full-screen-select
        "
        role="listbox"
      >
        <Login />
      </ul>
    </div>

    <button
      class="
        reset
        modal__close-btn modal__close-btn--outer
        js-modal__close
        js-tab-focus
      "
    >
      <svg class="icon icon--sm" viewBox="0 0 24 24">
        <title>Close modal window</title>
        <g
          fill="none"
          stroke="currentColor"
          stroke-miterlimit="10"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
        >
          <line x1="3" y1="3" x2="21" y2="21" />
          <line x1="21" y1="3" x2="3" y2="21" />
        </g>
      </svg>
    </button>
  </div>

  <div
    data-theme="dark"
    class="
      modal modal--animate-scale
      bg bg-opacity-99%
      flex flex-center
      padding-md
      js-modal
    "
    id="modal-register"
  >
    <div
      class="
        modal__content
        max-width-xs max-height-100%
        overflow-auto
        padding-md
        text-center
      "
      role="alertdialog"
      aria-labelledby="modal-select-title"
      aria-describedby=""
    >
      <p
        class="color-contrast-medium margin-bottom-xs"
        id="modal-select-title"
      ></p>

      <ul
        class="
          full-screen-select
          flex flex-column
          gap-xxs
          js-full-screen-select
        "
        role="listbox"
      >
        <SignUp />
      </ul>
    </div>

    <button
      class="
        reset
        modal__close-btn modal__close-btn--outer
        js-modal__close
        js-tab-focus
      "
    >
      <svg class="icon icon--sm" viewBox="0 0 24 24">
        <title>Close modal window</title>
        <g
          fill="none"
          stroke="currentColor"
          stroke-miterlimit="10"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
        >
          <line x1="3" y1="3" x2="21" y2="21" />
          <line x1="21" y1="3" x2="3" y2="21" />
        </g>
      </svg>
    </button>
  </div>
</template>

<script>
import Login from "@/components/Login.vue";
import SignUp from "@/components/SignUp.vue";

export default {
  name: "DrawerNavigation",
  components: {
    Login,
    SignUp,
  },
  mounted() {
    let frontEnd = document.createElement("script");
    frontEnd.setAttribute("src", "js/drawer-navigation.js");
    frontEnd.setAttribute("id", "drawer-navigation-js");

    document.body.appendChild(frontEnd);
  },
  destroyed() {
    document.getElementById("drawer-navigation-js").remove();
  },
};
</script>

<style lang="scss">
@use "../../node_modules/codyhouse-framework/main/assets/css/base/breakpoints"
  as *;
@use "../../node_modules/codyhouse-framework/main/assets/css/base/mixins" as *;

@use "../assets/css/custom-style/full-screen-select" as *;
@use "../assets/css/custom-style/drawer-navigation" as *;
</style>