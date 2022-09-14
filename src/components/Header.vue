<template>
  <header class="header">
    <div class="header-title__box header-cell">
      <h1 class="header-cell__text">ПРОИЗВОДСТВО ЦВЕТНЫХ МЕТАЛЛОВ И СПЛАВОВ</h1>
    </div>
    <nav class="wrapper header-nav">
      <Logo />
      <div class="header-nav__btn">
        <button class="nav-btn__call nav-call">
          <img class="nav-call__img" src="../img/call.png" alt="err_img" />
        </button>
        <button class="nav-btn__burger">burger</button>
      </div>
    </nav>
  </header>
</template>

<script>
import Logo from "./modules/logo.vue";

export default {
  components: {
    Logo,
  },
};
</script>

<style scoped lang="scss">
.header {
  &-cell {
    background-color: #2b323c;
    padding: 20px 20px;

    &__text {
      display: grid;
      justify-content: center;
      font-family: Roboto-Bold;
      font-weight: 700;
      font-size: 11px;
      color: #ffffff;
    }
  }
  &-nav {
    margin: 12px 0px;
    display: grid;
    align-items: center;
    grid-template-columns: 2fr 1fr;

    &__btn {
      display: grid;
      grid-template-columns: 40px 40px;
      gap: 10px;
      justify-content: end;
    }
  }
}
.nav {
  &-box {
    &__cell {
      display: flex;
      align-items: center;
      margin: 12px 0px 0px 0px;
    }
    &__subtitle {
      font-weight: 400;
      font-size: 10px;
    }
  }
  &-btn {
    &__call {
      display: grid;
      justify-items: center;
      align-items: center;
      width: 40px;
      height: 40px;
      border: 0px solid;
      background-color: #bf9d77;
      color: white;
    }
    &__burger {
      width: 40px;
      height: 40px;
      border: 0px solid;
      background-color: #983031;
      color: white;
    }
  }
}
</style>
