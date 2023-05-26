<script setup></script>

<template>
  <div class="mobile">
    <router-view class="router"></router-view>
  </div>
</template>

<style scoped>

.mobile {
  position: relative;
  display: none;
}

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

  .router {
    margin-top: -5em !important;
    padding: 0 20px !important;
    width: 100% !important;

    max-height: 38em !important;
    overflow-y: auto;
  }

  .mobile {
    margin: 80px auto;
    display: block;
    width: 320px;
  }

  .hero {
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
