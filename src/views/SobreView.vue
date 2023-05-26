<script setup>
import Profile from "../components/Profile.vue";
</script>

<template>
  <main>
    <Profile />

    <!-- Seção de Sobre -->
    <section>
      <p>
        Olá!! me chamo Guilherme Wilker e sou um entusiasta no Desenvolvimento
        Frontend, buscando constantemente me atualizar em novas tecnologias e
        tendências de mercado. <br />
        <br />

        Possuo vasta experiência no desenvolvimento web, desde a programação e o
        design de páginas, integrando APIs externas como Stripe, Mercado Pago e
        entre outras disponíveis. Familiaridade também com PWAs e SAPs
        garantindo a usabilidade e acessibilidade das aplicações. <br />
        <br />

        Além de ser <strong>mega apaixonado</strong> por Arte, NBA e Soundgarden
        <br />(torcedor assíduo do Celtics).
      </p>
    </section>
  </main>
</template>

<style scoped>
main {
  width: 600px;
  padding: 20px;
  display: flex;
  flex-direction: column;

  margin: 0 auto;
  width: 540px;
  background-color: #f8f1ec;
  padding: 0px 40px;
}

section {
  margin-bottom: 30px;
}

p {
  font-size: 14px;
  text-align: justify;
}
</style>
