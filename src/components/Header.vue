<template>
  <header>
    <router-link to="/">
      <h3 class="logo">Guilherme Wilker</h3>
    </router-link>

    <nav>
      <router-link to="/projetos">Projetos</router-link>
      <router-link to="/sobre">Sobre mim</router-link>
    </nav>

    <a
      href="https://www.linkedin.com/in/guilherme-wilker/"
      class="contact_button"
      >Let's Chat</a
    >

    <nav class="mobile_nav">
      <a href="/projetos">Projetos</a>
      <a href="/sobre">Sobre mim</a>
    </nav>
  </header>
</template>

<script setup></script>

<style scoped>
.mobile_nav {
  display: none;
}

header {
  position: relative;
  width: 100%;

  display: flex;
  justify-content: center;
  align-items: center;

  padding: 15px;

  gap: 350px;
  border-bottom: 2px solid #f8f1ec;
}

nav {
  display: flex;
  align-items: center;
  gap: 40px;
}

.logo {
  font-weight: bold;
}

.contact_button {
  padding: 12px 34px;
  border: 1px solid black;

  transition: 0.4s ease-in-out;
}

.contact_button:hover {
  background-color: #2c7ae0;
  color: white;
  border: 1px solid #2c7ae0;
}

@media (max-width: 1090px) {
  header {
    gap: 80px;
  }
}
@media (max-width: 700px) {
  header {
    gap: 30px;
  }
}

@media (max-width: 500px) {
  .contact_button {
    display: none;
  }

  nav {
    display: flex;
    font-size: 12px;
    gap: 12px;
  }

  nav a {
    background-color: #fce1a8;
    padding: 8px;
    border-radius: 2px;
  }
}

@media(max-width: 320px){
  header {
    gap: 10px;
  }
  .logo {
    font-size: 15px;
  }

  nav a {
   font-size: 12px;
   padding: 5px;
  }
}
</style>
