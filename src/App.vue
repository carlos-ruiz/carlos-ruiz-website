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
    --primary-text-color: #d3edea;
    --primary-text-color-inverse: #09333f;
    --primary-color: #009d9a;
    --secondary-color: #26f7b2;
    --background-color: #09333f;

    --font-1: 'DM Sans', sans-serif;
    --font-2: 'Roboto', sans-serif;
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

  h1, h2, h3, h4, h5 {
    font-family: var(--font-1);
  }

  header,
  body,
  footer {
    margin: 0;
    padding: 0;
    font-size: 1.6rem;
    font-family: var(--font-2);
  }

  #app {
    display: flex;
    flex-direction: column;
    height: 100%;
  }

  nav {
    background-color: var(--primary-color);
    padding: 16px;
    font-weight: 700;

    ul {
      display: flex;
      flex-direction: row;
      align-items: center;
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
      color: var(--primary-text-color);
      text-decoration: none;

      &:hover {
        color: var(--primary-text-color-inverse);
      }
    }
  }

  main.container {
    flex-grow: 1;
  }
</style>
