<template>
<div class="inner-block">
  <div class="vue-tempalte">
    <form>
      <h3>Sign Up</h3>

      <div class="form-group">
        <label>Full Name</label>
        <input type="text" class="form-control form-control-lg" />
      </div>

      <div class="form-group">
        <label>Email address</label>
        <input type="email" class="form-control form-control-lg" />
      </div>

       <div class="form-group">
        <label>Phone number</label>
        <input type="email" class="form-control form-control-lg" />
      </div>
        <div class="form-group-password">
      <div class="form-group">
        <label>Password</label>
        <input type="password" class="form-control form-control-lg"/>
      </div>
       <div class="form-group">
        <label>Confirm Password</label>
        <input type="password" class="form-control form-control-lg" />
      </div>
        </div>

      <button type="submit" class="login-btn btn-primary btn-lg btn-block">
       Sign Up
      </button>

      <p class="forgot-password text-right">
        Already registered
        <router-link style="font-size:16px; color:#2554ff" :to="{ name: 'login' }">sign in?</router-link>
      </p>
    </form>
  </div>
</div>
</template>

export default {
  data() {
    return {
      showPassword: false,
      password: null
    };
  },
  computed: {
    buttonLabel() {
      return (this.showPassword) ? "Hide" : "Show";
    }
  },
  methods: {
    toggleShow() {
      this.showPassword = !this.showPassword;
    }
  }
};
</script>
