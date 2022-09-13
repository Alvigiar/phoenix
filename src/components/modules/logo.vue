<template>
  <div class="logo">
    <img class="logo__img" src="../../img/logo.png" alt="err_img" />
    <span class="logo__title">ФЕНИКС</span>
    <span class="logo__subtitle"> Научно-производственное объединение </span>
  </div>
</template>

<script></script>

<style scoped lang="scss">
.logo {
    display: grid;
    gap: 4px 10px;
    align-items: center;
    justify-items: center;

  &__img {
    grid-column: 1;
  }
  &__title {
    width: 214px;
    grid-column: 2;
    font-family: Roboto-Black;
    font-size: 52px;
    color: #983031;
  }
  &__subtitle {
    grid-column: 1/3;
    width: 270px;
    font-family: Roboto-Regular;
    font-size: 13px;
    letter-spacing: 0.049em;
    color: #2b323c;
  }
}
</style>
