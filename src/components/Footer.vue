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
      <div class="disclaimer">
        Copyright &copy; {{ new Date().getFullYear() }} Carlos Ruiz
      </div>
    </div>
  </footer>
</template>

<style lang="less" scoped>
  footer {
    background-color: transparent;
    padding: 16px;
    text-align: center;

    nav {
      padding: 0;

      ul {
        justify-content: center;
      }
    }

    .disclaimer {
    }
  }
</style>
