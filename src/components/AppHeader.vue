<template>
    <header class="toolbar">
      <div class="toolbar__container">
        <img class="toolbar__logo" src="../assets/logo/logo.svg">
        <nav class="toolbar__nav nav">
          <a
            flat
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
  @import 'https://fonts.googleapis.com/css?family=Source+Sans+Pro&display=swap';
  @import 'https://fonts.googleapis.com/css?family=Overpass:100,100i,200,200i,300,300i,400,400i,600,600i,700,700i,800,800i,900,900i&display=swap';

  $emailColor: #8d8c8c;

  @mixin displayFlexCenter() {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  @mixin displayFlexBetween() {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  @mixin displayFlexAround() {
    display: flex;
    justify-content: space-around;
    align-items: center;
  }

  .toolbar {
    @include displayFlexCenter();
    background-color: #fff;
    height: 65px;
    width: 100%;
    position: fixed;
    z-index: 2;
    left: 50%;
    transform: translate(-50%, 0);

    &__container {
      @include displayFlexBetween();
      width: 930px;
    }

    &__logo {
      width: 135px;
      margin-right: 25px;
    }

    &__nav {
      @include displayFlexBetween();
      width: 455px;
      padding-bottom: 5px;

    }

  .nav__link {
    font-family: 'Source Sans Pro', sans-serif;
    font-size: 16px;
  }

  .user {
    @include displayFlexBetween();

    &__text {
      width: 140px;
    }

    &__name,
    &__email {
      font-family: 'Overpass', sans-serif;
      font-size: 13px;
      margin-bottom: 0;
      text-align: right;
    }

    &__email {
      color: $emailColor;
      font-size: 12px;
      font-weight: 100;
    }

    &__images {
      display: flex;
      justify-content: space-between;
      align-items: center;
      width: 80px;
      margin-left: 15px;
    }

    &__avatar {
      width: 40px;
      border-radius: 50%;
    }

    &__signout {
      width: 25px;
    }
  }
  }
</style>
