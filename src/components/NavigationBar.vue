<script setup lang="ts"></script>

<template>
  <header>
    <nav>
      <ul>
        <li>
          <router-link to="/" class="nav-icon"
            ><img src="@/assets/only-logo.svg" alt="site-logo"
          /></router-link>
        </li>
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/about">About</router-link></li>
        <li><router-link to="/contact">Contact</router-link></li>
      </ul>
    </nav>
  </header>
</template>

<style lang="less" scoped>
  header nav ul {
    img {
      max-height: 50px;
      svg {
        fill: var(--primary-text-color);
      }
    }

    .nav-icon:hover {
      border: 0;
    }
  }
</style>
