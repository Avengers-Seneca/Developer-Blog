<template>
  <form class="sign-up-form">
    <div class="text-component text-center margin-bottom-sm">
      <h1>Get started</h1>
      <p>
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. <br />
        Already have an account? <a href="#0">Login</a>
      </p>
    </div>

    <div class="grid gap-xs">
      <div class="col-12@xs">
        <button class="btn btn--subtle width-100%">
          <svg
            aria-hidden="true"
            class="icon margin-right-xxxs"
            viewBox="0 0 16 16"
          >
            <g>
              <path
                d="M15.3,0H0.7C0.3,0,0,0.3,0,0.7v14.7C0,15.7,0.3,16,0.7,16H8v-5H6V8h2V6c0-2.1,1.2-3,3-3 c0.9,0,1.8,0,2,0v3h-1c-0.6,0-1,0.4-1,1v1h2.6L13,11h-2v5h4.3c0.4,0,0.7-0.3,0.7-0.7V0.7C16,0.3,15.7,0,15.3,0z"
              ></path>
            </g>
          </svg>
          <span>Join using Facebook</span>
        </button>
      </div>
    </div>

    <p class="text-center margin-y-sm">or</p>

    <div class="margin-bottom-sm">
      <div class="grid gap-xs">
        <div class="col-6@md">
          <label class="form-label margin-bottom-xxxs" for="input-first-name"
            >First name</label
          >
          <input
            class="form-control width-100%"
            type="text"
            name="input-first-name"
            id="input-first-name"
          />
        </div>

        <div class="col-6@md">
          <label class="form-label margin-bottom-xxxs" for="input-last-name"
            >Last name</label
          >
          <input
            class="form-control width-100%"
            type="text"
            name="input-last-name"
            id="input-last-name"
          />
        </div>
      </div>
    </div>

    <div class="margin-bottom-sm">
      <label class="form-label margin-bottom-xxxs" for="input-email"
        >Email</label
      >
      <input
        class="form-control width-100%"
        type="email"
        name="input-email"
        id="input-email"
        placeholder="email@myemail.com"
      />
    </div>

    <div class="margin-bottom-md">
      <label class="form-label margin-bottom-xxxs" for="input-password"
        >Password</label
      >
      <input
        class="form-control width-100%"
        type="password"
        name="input-password"
        id="input-password"
      />
      <p class="text-xs color-contrast-medium margin-top-xxs">
        Minimum 6 characters
      </p>
    </div>

    <div class="margin-bottom-sm">
      <button class="btn btn--primary btn--md width-100%">Join</button>
    </div>

    <div class="text-center">
      <p class="text-xs color-contrast-medium">
        By joining, you agree to our <a href="#0">Terms</a> and
        <a href="#0">Privacy Policy</a>.
      </p>
    </div>
  </form>
</template>

<script>
export default {
    name: "SignUp"
}
</script>