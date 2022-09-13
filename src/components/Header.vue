<template>
  <header class="header">
    <div class="header-title__box title-box">
      <h1 class="title-box__text">ПРОИЗВОДСТВО ЦВЕТНЫХ МЕТАЛЛОВ И СПЛАВОВ</h1>
    </div>
    <div class="wrapper header-logo">
      <!-- <div class="header-logo__box logo-box">
        <img class="logo-box__img" src="../img/header-logo.png" alt="err_img" />
      </div> -->
      <Logo class="logo"/>
      <div class="header-logo__btn">
        <button class="logo-btn__call logo-call">
          <img class="logo-call__img" src="../img/call.png" alt="err_img" />
        </button>
        <button class="logo-btn__burger">burger</button>
      </div>
    </div>
  </header>
</template>

<script>
import Logo from "./modules/logo.vue";

export default {
  components: {
    Logo,
  }
}
</script>

<style scoped lang="scss">
.header {
  &-logo {
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
.title {
  &-box {
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
}
.logo {
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
