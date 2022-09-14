<template>
  <footer class="footer">
    <section class="wrapper footer__logo footer-logo">
      <Logo is-footer />
      <div class="footer-logo__subtitle">
        Вся продукция ООО «НПО «Феникс» проходит строжайший контроль сертифицированной
        лабораторией и соответствует требованиям ГОСТа и других стандартов качества.
      </div>
      <div class="footer-logo__subtext">
        Любое использование материалов с сайта запрещено без письменного разрешения
        администрации сайта.
      </div>
    </section>
    <section class="footer__background">
      <div class="wrapper footer__container">
        <Feedback />
        <div class="footer__socnet footer-socnet">
          <img class="footer-socnet__vk" src="../img/vk_icon.png" alt="err_img" />
          <img class="footer-socnet__yandex" src="../img/yandex_icon.png" alt="err_img" />
          <img class="footer-socnet__soc" src="../img/soc_icon.png" alt="err_img" />
        </div>
        <div class="footer__line"></div>
        <div class="footer__info footer-info">
          <a href="" class="footer-info__privacy">Политика конфиденциальности</a>
          <a href="" class="footer-info__requisites">Реквизиты</a>
          <div class="footer-info__text">
            Любое использование материалов с сайта запрещено без письменного разрешения
            администрации сайта.
          </div>
          <div class="footer-info__copyrights">Copyrights © 2022. Все права защищены</div>
        </div>
      </div>
    </section>
  </footer>
</template>

<script>
import Logo from "./modules/logo.vue";
import Feedback from "./modules/feedback.vue";

export default {
  components: {
    Logo,
    Feedback,
  },
};
</script>

<style scoped lang="scss">
.footer {
  display: grid;
  &-logo {
    &__subtitle {
      margin: 20px 0px 50px 0px;
      font-family: Roboto-Regular;
      font-size: 13px;
      line-height: 20px;
    }
    &__subtext {
      display: none;
      width: 275px;
      font-family: Roboto-Regular;
      font-size: 13px;
      line-height: 19px;
      letter-spacing: 0.05em;
      opacity: 0.4;
    }
  }
  &__background {
    padding: 48px 0px 50px 0px;
    display: grid;
    background-color: #2b323c;
    color: white;
  }

  &-box {
    display: grid;
    align-items: center;
    gap: 0px 10px;
    &__img {
      grid-column: 1;
    }
    &__email {
      grid-column: 2;
    }
  }
  &-work {
    grid-column: 2;
    display: flex;
    flex-wrap: wrap;
  }
  &-socnet {
    display: flex;
    gap: 0px 10px;
  }
  &__line {
    margin: 43px 0px 28px 0px;
    display: block;
    width: 100%;
    height: 1px;
    opacity: 30%;
    background-color: white;
  }
  &-info {
    display: grid;
    gap: 20px 0px;
    font-family: Roboto-Regular;
    font-size: 13px;
    line-height: 19px;
    &__privacy {
      text-decoration: none;
      color: #bf9d77;
    }
    &__requisites {
      text-decoration: none;
      color: #bf9d77;
    }
    &__copyrights {
      margin-top: 10px;
      opacity: 30%;
    }
  }
}

@media (min-width: 720px) {
  .footer {
    &-logo {
      grid-column: 1;
      &__subtitle {
        width: 275px;
        margin: 30px 0px 105px 0px;
      }
      &__subtext {
        display: block;
        line-height: 20px;
      }
    }
    &__background {
      grid-column: 2;
    }
    &-info {
      &__text {
        display: none;
      }
    }
  }
}
</style>
