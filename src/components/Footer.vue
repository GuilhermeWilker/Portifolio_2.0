<template>
  <footer>
    <p>© 2023 Guilherme Wilker. Todos os direitos reservados.</p>
  </footer>
</template>

<style scoped>
footer {
  padding-top: 15px;
}

footer p {
  text-align: left;
  margin-left: 20%;
  color: rgb(156, 156, 156);
}

@media (max-width: 500px) {
  footer p {
    margin-top: -4em;
    padding: 0 90px;
    text-align: center;
    margin-left: 0;
    font-size: 14px;
  }
}
</style>
