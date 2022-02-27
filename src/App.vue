<script setup lang="ts">
  // This starter template is using Vue 3 <script setup> SFCs
  // Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
  import NavigationBar from './components/NavigationBar.vue';
  import Footer from './components/Footer.vue';
</script>

<template>
  <NavigationBar />
  <main class="container">
    <router-view></router-view>
  </main>
  <Footer />
</template>

<style lang="less">
  :root {
    --primary-text-color: #000000;
    --primary-text-color-inverse: #ffffff;
    --primary-color: #42b983;
  }
  * {
    box-sizing: border-box;
  }

  html {
    font-size: 62.5%;
  }

  html, body {
    margin: 0;
    padding: 0;
    height: 100%;
  }

  header,
  body,
  footer {
    margin: 0;
    padding: 0;
    font-size: 1.6rem;
  }

  #app {
    display: flex;
    flex-direction: column;
    height: 100%;
  }

  nav {
    background-color: var(--primary-color);
    padding: 16px;

    ul {
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      list-style: none;
      padding: 0;

      li {
        padding: 0 8px;

        &:first-of-type {
          padding-left: 0;
        }
      }
    }

    a {
      color: var(--primary-text-color-inverse);
      text-decoration: none;

      &:hover {
        color: var(--primary-text-color);
      }
    }
  }

  main.container {
    flex-grow: 1;
  }
</style>
