<template>
  <div id="app">
    <header>

    </header>
    <navbar></navbar>

    <router-view/>

    <div class="spacer"></div>
    <footer>
      <span class="alert">** 可以分割 2D 的 png、nii 以及 nii.gz 格式的 *腮腺或甲状腺* 的超声（US）医学图像 **</span>
      <br>
      <span class="alert"></span>
      <!-- <br> -->
      Made by Bang
    </footer>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';

export default {
  name: "App",
  components: {
    navbar: Navbar
  }
};
</script>

<style>
#app {
  font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Oxygen,
    Ubuntu, Cantarell, Fira Sans, Droid Sans, Helvetica Neue, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-size: 16px;
  text-align: center;
  color: #2c3e50;

  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.spacer {
  flex: 1;
}

header {
  padding: 0.5rem 0;
}

.route {
  color: #7f8c8d;
  padding: 0rem 1rem;
}

body {
  margin: 0;
  background-color: #eee;
}

.github-corner:hover .octo-arm {
  animation: octocat-wave 560ms ease-in-out;
}

@keyframes octocat-wave {
  0%,
  100% {
    transform: rotate(0);
  }
  20%,
  60% {
    transform: rotate(-25deg);
  }
  40%,
  80% {
    transform: rotate(10deg);
  }
}

@media only screen and (max-width: 800px) {
  .github-corner:hover .octo-arm {
    animation: none;
  }
  .github-corner .octo-arm {
    animation: octocat-wave 560ms ease-in-out;
  }
}

footer {
  padding: 1rem;
  background-color: #efefef;
  text-align: center;
  color: #9fa9aa;
  font-weight: 200;
  font-size: 1rem;
}
.alert {
  color: #000000;
  font-weight: 400;
}
</style>
