<template>
  <div class="profile">
    <img src="/images/profile/avatar.png" alt="Guilherme Wilker" />
    <div class="profile_text-content">
      <img src="/images/icons/linkedin.png" alt="" />
      <a href="https://www.linkedin.com/in/guilherme-wilker" target="_blank">
        in/guilherme-wilker
      </a>
    </div>
  </div>
</template>

<style scoped>
.profile {
  padding: 50px 0;
  margin-inline: auto;
  display: flex;
  align-items: center;
  gap: 35px;

  width: 100%;
}

.profile_text-content {
  display: flex;
  align-items: center;
  gap: 12px;
}

a {
  font-size: 14px;
}

@media(max-width: 500px) {
  .profile {
   padding: 30px 0;
   gap: 12px;
  }

  a {
    font-size: 14px;
  }
}
</style>
