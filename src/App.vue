<script setup>
import { Transition } from "vue";
import HeaderVue from "./components/Header.vue";
import FooterVue from "./components/Footer.vue";
import { RouterLink, RouterView } from "vue-router";
import Mobile from "./components/Mobile.vue";

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
  <HeaderVue />
  <main>
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

    <div class="router-box">
      <router-view v-slot="{ Component }">
        <!-- <transition name="slide-up" mode="out-in"> -->
        <component :is="Component" />
        <!-- </transition> -->
      </router-view>
    </div>
  </main>

  <Mobile />

  <FooterVue />
</template>

<style scoped>
main {
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: center;

  gap: 30px;
  height: 80vh;
}

.router-box {
  height: 100% ;
}

.hero {
  width: 560px;
}

.hero_text-heading h4 {
  display: flex;
  align-items: center;

  gap: 15px;
  font-size: 20px;
}

.hero_text-heading h1 {
  font-size: 40px;
}
.hero_text-heading p {
  width: 500px;
  text-align: justify;
  margin-top: 16px;
  font-size: 14px;
}

.stacks {
  margin-top: 20px;
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
@media (max-width: 1370px) {
  main {
    height: 90vh;
  }
  .router-box {
    height: 100%;
  }
  footer {
    padding: 10px 0px;
  }
}

@media (max-width: 900px) {
  main {
    display: none;
  }
}
</style>
