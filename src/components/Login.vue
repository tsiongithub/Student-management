<template>
<div>
  
   <div class="inner-block">
      <h3>Sign in</h3>
  <div class="vue-tempalte">
    <form>
      <div class="form-group">
        <label>Email address</label>
        <input type="email" class="form-control form-control-lg" placeholder="example@gmail.com" />
      </div>

      <div class="form-group">
        <label>Password</label>
        <input type="password" class="form-control form-control-lg" placeholder="Enter your password" />
      </div>

      <button type="submit" class="login-btn btn btn-primary btn-lg btn-block">
        Login
      </button>

      <p class="forgot-password text-center mt-2 mb-4">
        <router-link to="/forgot-password">Forgot password ?</router-link>
      </p>
      <div style="float:left; width: 44%;"><hr/></div>
<div style="float:right; width: 49%;"><hr/></div>
  <p>OR</p>
      <div class="social-icons">
        <ul>
          <li>
            <a href="#"><i class="fa fa-google"></i></a>
          </li>
          <li>
            <a href="#"><i class="fa fa-facebook"></i></a>
          </li>
          <li>
            <a href="#"><i class="fa fa-twitter"></i></a>
          </li>
        </ul>
      </div>
    </form>
  </div>
  </div>
  <p class="forgot-password text-center">
        Don't have any acccount
        <router-link style="font-size:16px ;color:#2554ff" :to="{ name: 'signup' }">? Sign Up</router-link>
      </p>
  
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>
