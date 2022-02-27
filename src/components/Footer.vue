<template>
  <footer>
    <div class="container">
      <nav>
        <ul>
          <li><a href="#">Términos y condiciones</a></li>
          <li><a href="#">Política de privacidad</a></li>
          <li><a href="#">Contáctanos</a></li>
        </ul>
      </nav>
      <div class="social">Social icons</div>
      <div class="disclaimer">Copyright &copy; {{new Date().getFullYear()}} Carlos Ruiz</div>
    </div>
  </footer>
</template>

<style lang="less" scoped>
  footer {
    background-color: #42b983;
    padding: 16px;

    nav {
      padding: 0;
    }
  }
</style>
