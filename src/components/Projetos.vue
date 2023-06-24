<template>
  <section class="project_section">
    <!-- PHocket -->
    <div class="card">
      <div class="img-container">
        <img src="/projetos/phocket.png" alt="" />
      </div>

      <div class="project_title-box">
        <h3 class="project_title">PHocket</h3>

        <div class="stacks">
          <span class="bullet-stack php">PHP</span>
          <span class="bullet-stack javascript">Javascript</span>
          <span class="bullet-stack">CSS</span>
        </div>
      </div>

      <p class="project_description">
        <span class="small-title">Phocket 🪙</span> é uma carteira virtual para
        monitoramento financeiro. Ajudando os usuários a terem controle sobre
        sua rentabilidade e despesas.
        <br />
      </p>

      <a
        href="https://github.com/GuilhermeWilker/Phocket"
        target="_blank"
        class="project_button"
        >Repositório</a
      >
    </div>

    <!-- Partager Player -->
    <div class="card">
      <div class="img-container">
        <img src="/projetos/partager-player.png" alt="" />
      </div>

      <div class="project_title-box">
        <h3 class="project_title">Partager Player</h3>

        <div class="stacks">
          <span class="bullet-stack vue">Vue</span>
          <span class="bullet-stack">CSS</span>
          <span class="bullet-stack firebase">Firebase</span>
        </div>
      </div>

      <p class="project_description">
        <span class="small-title">Partager Player 🎧</span> é uma PWA de música
        compartilhada, com ele tu pode curtir as músicas dos seus amigos, postar
        as suas músicas favoritas e ainda deixar comentários sobre cada uma
        delas!
        <br />
      </p>

      <a
        href="https://partagerpage.netlify.app/"
        target="_blank"
        class="project_button"
        >Acessar</a
      >
    </div>

    <!-- Mind On -->
    <div class="card">
      <div class="img-container">
        <img src="/projetos/mind-on.png" alt="" />
      </div>

      <div class="project_title-box">
        <h3 class="project_title">Mind On</h3>

        <div class="stacks">
          <span class="bullet-stack vue">Vue</span>
          <span class="bullet-stack">CSS</span>
        </div>
      </div>

      <p class="project_description">
        <span class="small-title">Mind on 🧠</span> é um web aplicativo para
        criação de mapas mentais. Facilitando o processo de absorção de conteúdo
        ou até mesmo no desenvolvimento de novas idéias, facilitando a
        compreensão e a organização de informações.
        <br />
      </p>

      <a
        href="https://mindon-page.netlify.app/"
        target="_blank"
        class="project_button"
        >Acessar</a
      >
    </div>

    <!-- Todo Today -->
    <div class="card">
      <div class="img-container">
        <img src="/projetos/todo-today.png" alt="" />
      </div>

      <div class="project_title-box">
        <h3 class="project_title">Todo Today</h3>

        <div class="stacks">
          <span class="bullet-stack javascript">Javascript</span>
          <span class="bullet-stack">CSS</span>
        </div>
      </div>

      <p class="project_description">
        Ambiente de estudos com as principais funcionalidades para auxiliar em
        atividades acadêmicas, ideal para estudantes. Simples e funcional,
        <span class="small-title">Todo Today</span> traz as principais
        características para gerenciar suas atividades de estudos ou trabalho.
        Listando tarefas, utilizando o pomodoro ou criando anotações!
      </p>

      <a
        href="https://todotoday-page.netlify.app/"
        target="_blank"
        class="project_button"
        >Acessar</a
      >
    </div>

    <!-- Ask.ME -->
    <div class="card">
      <div class="img-container">
        <img src="/projetos/ask-me.png" alt="" />
      </div>

      <div class="project_title-box">
        <h3 class="project_title">Ask Me</h3>

        <div class="stacks">
          <span class="bullet-stack node">Node</span>
          <span class="bullet-stack mysql">MySQL</span>
        </div>
      </div>

      <p class="project_description">
        Comunidade de perguntas e respostas, criando interações entre os
        usuários de forma anônima e de temas livres (dado o supervisionamento da
        administração).
      </p>

      <a
        href="https://www.linkedin.com/feed/update/urn:li:activity:7006646867572715520/"
        target="_blank"
        class="project_button"
        >Acessar</a
      >
    </div>

    <!-- Luminária Livrolas -->
    <div class="card">
      <div class="img-container">
        <img src="/projetos/luminaria-livrolas.png" alt="" />
      </div>

      <div class="project_title-box">
        <h3 class="project_title">Luminária Livrolas</h3>

        <div class="stacks">
          <span class="bullet-stack javascript">Javascript</span>
        </div>
      </div>

      <p class="project_description">
        Ambiente de leitura virtual, aconchegante e clean. Facilitando e
        deixando a leitura do usuário menos maçante durante suas viagens
        literárias.
      </p>

      <a
        href="https://guilhermewilker.github.io/luminaria-livrolas/"
        target="_blank"
        class="project_button"
        >Acessar</a
      >
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
.project_section {
  margin-top: 15em;
  height: 100vh;
  width: 100%;
}

.card {
  margin-top: 25px;
  padding: 20px 0;
  display: flex;

  flex-direction: column;
}

.project_title-box {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin: 10px 0;
}

.project_title {
  font-size: 24px;
  padding-right: 30px;
}

.small-title {
  font-weight: 500;
}

span {
  font-weight: 500;
}

.stacks {
  display: flex;
  align-items: center;
  gap: 8px;
}

.project_description {
  text-align: justify;
  font-size: 15px;
  font-weight: 400;
}

.project_button {
  background-color: rgb(26, 26, 26);
  margin-inline-start: auto;
  text-align: center;

  margin-top: 12px;
  color: white;
  border: none;

  cursor: pointer;
  padding: 15px;
  width: 150px;

  font-size: 14px;
  transition: 0.5s ease-in-out;
}

.project_button:hover {
  background-color: rgb(15, 14, 14);
}

.img-container img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 8px;
}

.img-container {
  width: 100%;
  height: 230px;
}

@media (max-width: 1370px) {
  .project_section {
    margin-top: 8em;
  }

  .project_title {
    font-size: 20px;
    padding-right: 30px;
  }
  .bullet-stack {
    font-size: 13px;
  }

  .project_description {
    text-align: justify;
    font-size: 14px;
    font-weight: 400;
  }

  .project_button {
    background-color: rgb(26, 26, 26);
    margin-inline-start: auto;
    text-align: center;

    margin-top: 8px;
    color: white;
    border: none;

    cursor: pointer;
    padding: 12px;
    width: 150px;

    border-radius: px;
    font-size: 12px;
    transition: 0.5s ease-in-out;
  }

  .project_button:hover {
    background-color: rgb(15, 14, 14);
  }

  .img-container img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 8px;
  }

  .img-container {
    width: 100%;
    height: 220px;
  }
}

@media (max-width: 900px) {

  .project_section {
    margin-top: 1em;
  }

  .project_title-box {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin: 10px 0;
  }

  .project_title {
    font-size: 18px;
    padding-right: 5px;
  }
  .bullet-stack:last-child {
    display: none;
  }

  .project_description {
    text-align: justify;
    font-size: 14px;
    font-weight: 400;
  }

  .project_button {
    background-color: rgb(26, 26, 26);
    margin-inline-start: auto;
    text-align: center;

    margin-top: 8px;
    color: white;
    border: none;

    cursor: pointer;
    padding: 12px;
    width: 150px;

    border-radius: px;
    font-size: 12px;
    transition: 0.5s ease-in-out;
  }

  .project_button:hover {
    background-color: rgb(15, 14, 14);
  }

  .img-container img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 8px;
  }

  .img-container {
    width: 100%;
    height: 220px;
  }
}
</style>
