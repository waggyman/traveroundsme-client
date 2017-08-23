<template>
<div class="tv-login-page" style="padding-bottom: 72px; padding-top: 36px;">
  <div class="columns is-centered">
    <div class="column">
      <p class="tv-header">TraveroundsMe</p>
    </div>
  </div>
  <div class="columns  m-10 is-centered">
    <div class="column tv-description is-one-quarter">
      <p>
        Discover New Place, New Foods, New Culture, and New Experience.
      </p>
    </div>
  </div>
  <div class="columns is-centered">
    <div class="column is-one-quarter tv-login-container">
      <div class="field tv-centered">
          <label class="label light-label">TraveroundsMe - Login</label>
      </div>
      <div>
        <div class="field">
          <label class="label light-label">Email</label>
          <div class="control">
            <input class="input" v-model="email" type="email" name="email" placeholder="Email">
          </div>
        </div>
        <div class="field">
          <label class="label light-label">Password</label>
          <div class="control">
            <input class="input" v-model="password" type="password" placeholder="Password">
          </div>
        </div>
        <div style="padding-top: 25px;">
            <a href="#" class="register-link">Didn't have account, signup for free</a>
            <button @click="submit" class="button tv-button tv-primary pull-right">Submit</button>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
import axios from 'axios'
export default {
  name: 'login',
  data () {
    return {
      email: '',
      password: ''
    }
  },
  methods: {
    async submit () {
      let res = await axios.post('oauth/token', {
        'grant_type': 'password',
        'client_id': 2,
        'client_secret': 'v1Ytf1FcW53K5agJEQxxpj25ykm2beNnDN3BdM8j',
        'username': this.email,
        'password': this.password,
        'scope': '*'
      })

      console.log(res)
    }
  }
}
</script>

<style>
  .tv-login-page {
    background: linear-gradient(rgba(0,0,0,0.4),rgba(0,0,0,0.4)),
    url('https://static.pexels.com/photos/220444/pexels-photo-220444.jpeg') center center no-repeat;
  }
  .tv-container {
    padding: 10px 20px;
  }
  .tv-description {
    color: #f5f5f5;
    font-size: 18px;
    font-weight: 700;
    text-align: center
  }
  .tv-centered {
    text-align: center;
  }
  .tv-login-container {
    padding-top: 30px;
    padding-bottom: 30px;
    background-color: rgba(0, 0, 0, 0.6);
    margin: 30px 5px;
    box-shadow: 1px 2px 10px #000;
  }
  .register-link {
    float: left;
    margin-top: 18px;
    font-size: 12px;
    display: block;
    color: #00B467;
    text-decoration: underline;
  }
  .pull-right {
    display: block;
    float: right !important;
  }
  .light-label {
    color: #f5f5f5 !important;
  }
  .tv-header {
    color: #f5f5f5;
    font-size: 46px;
    font-weight: 700;
    text-align: center
  }
</style>
