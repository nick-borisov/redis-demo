<template>
  <header class="header">
    <div class="header__logo">
      <span class="header__logo-image" v-if="logoImage">
        <img :src="logoImage" alt=""/>
      </span>
      <span class="header__logo-text text-h3">
        <span class="header__logo-title">
          {{ logoTitle }}
        </span>
        <span class="header__logo-subtitle">
          {{ logoSubtitle }}
        </span>
      </span>
    </div>

    <div class="header__user">
      <span class="header__user-image">
        <img :src="userPhoto" alt="">
      </span>
      <span class="header__user-text">
        <span class="header__user-name">
          {{ userName }}
        </span>
        <span class="header__user-email text-h4">
          {{ userEmail }}
        </span>
      </span>
    </div>
    <div class="header__nav">
      <button type="button" class="header__nav-control">
        <img src="../../assets/img/icon/uil-log-out.svg">
      </button>
    </div>
  </header>
</template>

<script>
  export default {
    name: 'SiteHeader',
    props: {
      logoImage: String,
      logoTitle: String,
      logoSubtitle: String,
      userEmail: String,
      userName: String,
      userPhoto: String,
    },
  }
</script>
