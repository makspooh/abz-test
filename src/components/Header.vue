<template>
    <header class="toolbar">
      <div class="toolbar__container">
        <img class="toolbar__logo" src="../assets/logo/logo.svg">
        <nav class="toolbar__nav nav">
          <a
            v-for="link of links"
            :key="link"
            class="nav__link"
          >{{ link }}</a>
        </nav>
        <div class="toolbar__user user">
          <div class="user__text">
            <p class="user__name">Superstar</p>
            <p class="user__email">Superstar@gmail.com</p>
          </div>
          <div class="user__images">
            <img class="user__avatar" src="../assets/imgs/user-superstar-2x.jpg" alt="">
            <img class="user__signout" src="../assets/icons/sign-out.svg" alt="">
          </div>
        </div>
      </div>
    </header>
</template>

<script>
  export default {
    data: () => ({
      links: [
        'About me',
        'Relationships',
        'Requirements',
        'Users',
        'Sign Up'
      ],
    })
  }
</script>

<style lang="scss">
  @import '../scss/style';
</style>