<template>
  <div id="app">
      <navbar></navbar>
      <router-view></router-view>
      <nav-footer></nav-footer>
  </div>
</template>

<script>
import Navbar from '@/components/partials/Navbar'
import Footer from '@/components/partials/Footer'
export default {
  name: 'app',
  components: {
    navbar: Navbar,
    navFooter: Footer
  }
}
</script>

<style>
html {
  overflow-y: auto !important;
  min-height: 660px;
}
@import '../node_modules/bulma/css/bulma.css';
@import url('https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css');
body {
  margin: 0;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

main {
  text-align: center;
  margin-top: 40px;
}

header {
  margin: 0;
  height: 56px;
  padding: 0 16px 0 24px;
  background-color: #35495E;
  color: #ffffff;
}

header span {
  display: block;
  position: relative;
  font-size: 20px;
  line-height: 1;
  letter-spacing: .02em;
  font-weight: 400;
  box-sizing: border-box;
  padding-top: 16px;
}
.tv-primary {
  background-color: #00B467;
  color: #f5f5f5;
}
.tv-primary:hover {
  background-color: #0b9258;
  color: #f5f5f5;
}
.m-10 {
  margin-top: 10px;
}
.mb-0 {
  margin-bottom: 0 !important;
}
.tv-header {
    color: #f5f5f5;
    font-size: 46px;
    font-weight: 700;
    text-align: center
  }
  .pull-left {
    float: left !important;
  }
  .tv-text-left {
    text-align: left !important;
  }
  .tv-text-center {
    text-align: center !important;
  }
  .tv-form-control {
    width: 100%;
    padding: 8px 36px;
    line-height: 16px;
    font-size: 14px;
  }
  .tv-form-inline-icon {
    position: absolute;
    top: 0;
    color: #00B467;
    width: 2.25em !important;
    height: 2.25em !important;
  }
</style>
