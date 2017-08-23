<template>
  <nav class="tv-navbar">
    <div class="tv-container-fluid">
      <h4 class="tv-navbar-label">TraveroundsMe</h4>
      <ul class="tv-nav">
        <li>
          <router-link to="/">Home</router-link>
        </li>
        <li>
          <router-link to="/login">Login</router-link>
        </li>
        <li>
          <a @click="logout">Logout</a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'navbar',
  methods: {
    logout () {
      console.log('process logout')
      localStorage.removeItem('access_token')
      this.$router.go('/')
    }
  }
}
</script>

<style>
  .tv-navbar-label {
    margin: 0;
    float: left;
    padding: 15px;
    color: #f5f5f5;
  }
  .tv-navbar {
    list-style-type: none;
    background-color: #00B467;
    min-height: 50px;
    position: relative;
  }
  .tv-nav {
    padding: 0;
    list-style: none;
    margin: 0;
    float: right;
  }
  .tv-nav > li {
    display: inline-block;
    position: relative;
  }
  .tv-nav > li > a {
    position: relative;
    display: block;
    line-height: 20px;
    padding: 15px 15px;
    text-decoration: none;
    color: #f5f5f5
  }
</style>
