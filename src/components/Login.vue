<template>
     <form class="login-form">
    <div class="text-component text-center margin-bottom-sm">
      <h1>Log in</h1>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
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
                d="M16,8.048a8,8,0,1,0-9.25,7.9V10.36H4.719V8.048H6.75V6.285A2.822,2.822,0,0,1,9.771,3.173a12.2,12.2,0,0,1,1.791.156V5.3H10.554a1.155,1.155,0,0,0-1.3,1.25v1.5h2.219l-.355,2.312H9.25v5.591A8,8,0,0,0,16,8.048Z"
              ></path>
            </g>
          </svg>
          <span>Login with Facebook</span>
        </button>
      </div>
    </div>

    <p class="text-center margin-y-sm">or</p>

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

    <div class="margin-bottom-sm">
      <div class="flex justify-between margin-bottom-xxxs">
        <label class="form-label" for="input-password">Password</label>
        <span class="text-sm"><a href="#0">Forgot?</a></span>
      </div>

      <input
        class="form-control width-100%"
        type="password"
        name="input-password"
        id="input-password"
      />
    </div>

    <div class="margin-bottom-sm">
      <button class="btn btn--primary btn--md width-100%">Login</button>
    </div>

    <div class="text-center">
      <p class="text-sm">Don't have an account? <a href="#0">Get started</a></p>
    </div>
  </form>
</template>

<script>
export default {
    name: "Login"
}
</script>