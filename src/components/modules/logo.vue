<template>
  <div class="logo" v-bind:class="{ logo_footer: isFooter }">
    <div class="logo__cell">
      <img class="logo__img" src="../../img/logo.png" alt="err_img" />
      <span class="logo__title">ФЕНИКС</span>
    </div>
    <div class="logo__subtitle">Научно-производственное объединение</div>
  </div>
</template>

<script>
export default {
  props: {
    isFooter: {
      type: Boolean,
      default: false,
    },
  },
};
</script>

<style scoped lang="scss">
.logo {
  max-width: 158px;
  display: flex;
  flex-direction: column;

  &__cell {
    align-items: center;
    justify-content: space-between;
    display: flex;
    gap: 6px;
  }

  &__img {
    width: 26px;
    height: 28px;
  }
  &__title {
    font-family: Roboto-Black;
    font-size: 30px;
    color: #983031;
  }
  &__subtitle {
    font-family: Roboto-Regular;
    font-size: 7.60741px;
    letter-spacing: 0.05em;
    color: #2b323c;
  }
  &.logo_footer {
    margin-top: 40px;
    max-width: 270px;
    align-items: center;
    .logo__box {
      gap: 0px 10px;
      // gap: 0px 10px;
    }
    .logo__img {
      width: 45px;
      height: 50px;
    }
    .logo__title {
      font-size: 52px;
    }
    .logo__subtitle {
      font-size: 13px;
      letter-spacing: 0.5px;
    }
  }
}

@media (min-width: 720px) {
  .logo {
    &.logo_footer {
      margin-top: 75px;
    }
  }
}
</style>
