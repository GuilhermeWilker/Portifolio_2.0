<script setup>

const stacks = [
  { src: "/images/stacks/javascript.png", alt: "JavaScript" },
  { src: "/images/stacks/vue.js.png", alt: "Vue.js" },
  { src: "/images/stacks/nuxt.png", alt: "Nuxt.js" },
  { src: "/images/stacks/react.js.png", alt: "React.js" },
  { src: "/images/stacks/sass.png", alt: "Sass" },
  { src: "/images/stacks/figma.png", alt: "Figma" },
  { src: "/images/stacks/firebase.png", alt: "Firebase" },
  { src: "/images/stacks/node.js.png", alt: "Node.js" },
  { src: "/images/stacks/php.png", alt: "PHP" },
  { src: "/images/stacks/sql.png", alt: "SQL" },
];
</script>

<template>
  <main></main>

  <div class="hero">
    <div class="hero_text-heading">
      <h4>
        Olá! Me chamo <span class="bullet">UX~UI</span
        ><span class="bullet">Front-end</span
        ><span class="bullet">Freelancer</span>
      </h4>
      <h1>Guilherme Wilker</h1>

      <p>
        Entusiasta no Desenvolvimento Frontend buscando constantemente me
        atualizar em novas tecnologias e tendências de mercado.
      </p>
    </div>

    <div class="stacks">
      <div class="hab_img-container">
        <img
          v-for="stack in stacks"
          :key="stack.src"
          :src="stack.src"
          :alt="stack.alt"
        />
      </div>
    </div>
  </div>
</template>

<style scoped>
.hero {
  display: none;
}
main {
  display: block;
  font-weight: 600;
  text-align: center;
  text-decoration: underline;

  width: 600px;
  height: 100%;

  padding: 20px;
  display: flex;
  flex-direction: column;

  margin: 0 auto;
  width: 540px;
  background-color: #f8f1ec;
  padding: 0px 40px;

  background-image: url("/images/f415a29771d6272bc9f7f95fd13eb74a.jpg");
  background-position: center;
  background-size: cover;

  filter: grayscale(1);
  transition: 0.8s ease-in-out;
}

main:hover {
  filter: grayscale(0);
  display: block;
  cursor: pointer;
  color: white;
}

/* MOBILE */

@media (max-width: 900px) {
  .mobile {
    margin: 80px auto;
    display: block;
    width: 400px;
  }

  .hero {
    width: 560px;
  }

  .hero_text-heading h4 {
    display: flex;
    align-items: center;

    gap: 15px;
    font-size: 18px;
  }

  .hero_text-heading h1 {
    font-size: 30px;
  }
  .hero_text-heading p {
    width: 80%;
    text-align: justify;
    margin-top: 16px;
    font-size: 14px;
  }

  .stacks {
    margin-top: 20px;
  }

  h4 .bullet {
    font-size: 11px;
  }

  .bullet:last-child {
    display: none;
  }

  .hab_img-container {
    margin-top: 30px;
    width: 450px;
    display: flex;
    align-items: center;
    flex-wrap: wrap;

    gap: 25px;
  }

  .hab_img-container img {
    width: 56px;
  }

  .hab_img-container img:first-child {
    width: 70px;
  }

  .hab_img-container img:nth-child(9) {
    width: 70px;
  }
}

@media (max-width: 500px) {
  .mobile {
    margin: 80px auto;
    display: block;
    width: 320px;
  }

  .hero {
    display: block;
    width: 100%;
  }

  .hero_text-heading h4 {
    display: flex;
    align-items: center;

    gap: 15px;
    font-size: 18px;
  }

  .hero_text-heading h1 {
    font-size: 30px;
  }
  .hero_text-heading p {
    width:100%;
    text-align: justify;
    margin-top: 16px;
    font-size: 14px;
  }

  h4 .bullet {
    font-size: 11px;
  }

  .bullet:first-child {
    display: none;
  }

  .bullet:last-child {
    display: none;
  }

  .hab_img-container {
    margin-top: 45px;
    width: 320px;
    display: flex;
    align-items: center;
    flex-wrap: wrap;

    gap: 25px;
  }

  .hab_img-container img {
    width: 56px;
  }

  .hab_img-container img:first-child {
    width: 70px;
  }

  .hab_img-container img:nth-child(9) {
    width: 70px;
  }
}
</style>
