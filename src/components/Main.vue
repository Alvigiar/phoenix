<template>
  <section class="wrapper lab">
    <h1 class="lab__title">СОБСТВЕННАЯ ЛАБОРАТОРИЯ</h1>
    <div class="lab__text">
      ООО НПО "Феникс" обладает собственной, аккредитированной и сертифицированной
      лабораторией по определению химического состава черных и цветных металлов и их
      сплавов.
    </div>
    <BtnDetails />
    <button class="lab"></button>
    <div class="lab-slider">
      <div class="lab-slider__line">
        <span class="lab-slider__line-content"></span>
        <span class="lab-slider__line-content"></span>
        <span class="lab-slider__line-content"></span>
      </div>
      <BtnArrow />
    </div>
  </section>

  <section class="wrapper prod">
    <h1 class="prod-title">Производство нашей компании</h1>
    <h2 class="prod-subtitle">Цветные металлы и сплавы</h2>
    <div class="prod-text">
      Из цветных металлов в чистом виде и в виде сплавов широко используются: цинк,
      бронза, олово, различные припои и прочее.
    </div>
    <div class="prod-slider">
      <div class="prod-slider__box prod-box">
        <h3 class="prod-box__title">
          Припои на основе индия
          <br />
          ПОИн10, ПОИн52, ПОИн90 и другие
        </h3>
        <Line />
        <div class="prod-box__text slider-box__text">
          фольга, пруток, проволока, слиток
        </div>
      </div>
      <div class="prod-slider__btn prod-btn slider-btn">
        <button class="prod-btn__all slider-btn__all">Вся продукция</button>
        <BtnArrow />
      </div>
    </div>
  </section>

  <section class="services">
    <div class="wrapper">
      <h1 class="services-title">Наши услуги</h1>
      <h2 class="services-subtitle">Что мы делаем для Вас</h2>
      <div class="services-text">
        Наше предприятие предоставляет своим партнёрам все необходимые услуги
      </div>
      <div class="services-slider">
        <div class="services-slider__content services-content">
          <div class="services-content__img">img</div>
          <div class="services-content__box services-box">
            <h3 class="services-box__title">
              Доставка продукции собственным автотранспортом
            </h3>
            <Line />
            <div class="services-box__text">
              ООО НПО «Феникс» предоставляет услуги по доставке продукции до покупателя.
              Мы беспечиваем оперативную доставку нашей
            </div>
            <BtnDetails />
          </div>
        </div>
        <BtnArrow />
      </div>
    </div>
  </section>

  <section class="wrapper partners">
    <h1 class="partners__title">Наши партнёры</h1>
    <h2 class="partners__subtitle">Партнёры НПО «ФЕНИКС»</h2>
    <div class="partners__text">
      Наша компания успешно развивается на рынке металлов и сплавов, активно участвует в
      гос закупках и является надежным поставщиком.
    </div>
    <div class="partners__slider partners-slider">
      <img src="" alt="err_img" class="partners-slider__img" />
      <BtnArrow />
    </div>
  </section>

  <section class="blog">
    <div class="wrapper">
      <h1 class="blog__title">Блог</h1>
      <h2 class="blog__subtitle">Последние статьи</h2>
      <article class="blog__article blog-article">
        <img class="blog-article__img" src="../img/met.png" alt="err_img" />
        <h3 class="blog-article__title">Вторая жизнь металлолома</h3>
        <ImgInfo />
        <Line />
        <div class="blog-article__text">
          Сдача металлолома позволяет многим организациям, не только навести порядок на
          своей территории, но и получить весомый доход.
        </div>
        <BtnDetails />
      </article>
      <article class="blog__article blog-article">
        <img class="blog-article__img" src="../img/colormet.png" alt="err_img" />
        <h3 class="blog-article__title">
          Цветной металлопрокат: особенности и разновидности
        </h3>
        <ImgInfo />
        <Line />
        <div class="blog-article__text">
          Цветной металлопрокат применяют сегодня в машиностроении и электронике, военном
          производстве и строительстве, авиастроении и не только.
        </div>
        <BtnDetails />
      </article>

      <div class="blog__list blog-list">
        <article class="blog-list__item blog-item">
          <h3 class="blog-item__title">Национальный сертификат лидера отрасли России</h3>
          <ImgInfo />
        </article>
        <div class="blog-list__line"></div>
        <article class="blog-list__item blog-item">
          <h3 class="blog-item__title">
            Цветной металлопрокат: особенности и разновидности
          </h3>
          <ImgInfo />
        </article>
        <div class="blog-list__line"></div>
        <article class="blog-list__item blog-item">
          <h3 class="blog-item__title">
            Вторая жизнь металлолома
            <ImgInfo />
          </h3>
        </article>
        <div class="blog-list__line"></div>
        <article class="blog-list__item blog-item">
          <h3 class="blog-item__title">Национальный сертификат лидера отрасли России</h3>
          <ImgInfo />
        </article>
      </div>
    </div>
  </section>

  <Article />
</template>

<script>
import Line from "./modules/line.vue";
import BtnArrow from "./modules/button-arrow.vue";
import BtnDetails from "./modules/button-detailed.vue";
import ImgInfo from "./modules/img-info.vue";

export default {
  name: "Main",
  components: {
    Line,
    BtnArrow,
    BtnDetails,
    ImgInfo,
  },
};
</script>

<style scoped lang="scss">
.lab {
  padding-top: 39px;
  // background-color: #2b323c;
  background-image: url("../img/self.png");
  background-repeat: no-repeat;
  background-size: cover;
  color: #ffffff;

  &__title {
    font-family: Roboto-Black;
    margin-bottom: 20px;
    font-weight: 900;
    font-size: 36px;
    line-height: 47px;
  }

  &__text {
    font-family: Roboto-Regular;
    margin-bottom: 40px;
    font-weight: 400;
    font-size: 16px;
    line-height: 24px;
  }
  &-slider {
    display: grid;
    align-items: center;
    grid-template-columns: 2fr 1fr;

    &__line {
      display: grid;
      grid-template-columns: repeat(3, 25px);
      gap: 10px;
    }

    &__line-content {
      display: block;
      width: 25px;
      height: 1px;
      gap: 5px;
      background-color: white;
    }
  }
}

.prod {
  margin-top: 37px;

  &-title {
    font-family: Roboto-Black;
    margin-bottom: 10px;
    font-size: 28px;
    line-height: 36px;
    color: #2b323c;
  }

  &-subtitle {
    font-family: Roboto-Bold;
    margin-bottom: 20px;
    font-size: 16px;
    color: #bf9d77;
  }

  &-text {
    font-family: Roboto-Regular;
    margin-bottom: 31px;
    font-size: 16px;
    line-height: 24px;
  }

  &-box {
    display: grid;
    padding: 190px 40px 30px 30px;
    background-color: #2b323c;
    color: white;

    &__title {
      font-family: Roboto-Bold;
      font-size: 16px;
      line-height: 24px;
    }

    &__text {
      font-family: Roboto-Regular;
      font-size: 16px;
      line-height: 24px;
    }
  }

  &-slider {
    &__btn {
      height: 50px;
      margin: 31px 0px 50px 0px;
      display: grid;
      justify-content: space-between;
      grid-template-columns: 150px 120px;
    }
  }

  &-btn {
    &__all {
      width: 149px;
      height: 60px;
      border: 0px solid;
      font-family: Roboto-Regular;
      font-size: 16px;
      background-color: #bf9d77;
      color: white;
    }
  }
}

.services {
  padding: 37px 0px 50px 0px;
  background-color: #f9f9f9;

  &-title {
    font-family: Roboto-Black;
    margin-bottom: 10px;
    font-size: 28px;
  }

  &-subtitle {
    font-family: Roboto-Bold;
    margin-bottom: 20px;
    font-size: 16px;
    color: #bf9d77;
  }

  &-text {
    font-family: Roboto-Regular;
    margin-bottom: 30px;
    font-size: 16px;
    line-height: 24px;
  }

  &-content {
    margin-bottom: 30px;
    background-color: white;

    &__img {
      height: 180px;
      display: block;
      background-color: black;
      color: white;
    }
  }

  &-box {
    padding: 20px;

    &__title {
      font-family: Roboto-Bold;
      font-weight: 700;
      font-size: 16px;
      line-height: 24px;
    }

    &__text {
      font-family: Roboto-Regular;
      margin-bottom: 20px;
      font-weight: 400;
      font-size: 12px;
      line-height: 18px;
    }
  }
}

.partners {
  margin: 36px 0px 50px 0px;

  &__title {
    font-family: Roboto-Black;
    margin-bottom: 10px;
    font-size: 28px;
  }

  &__subtitle {
    font-family: Roboto-Bold;
    margin-bottom: 20px;
    font-size: 16px;
    color: #bf9d77;
  }

  &__text {
    font-family: Roboto-Regular;
    margin-bottom: 30px;
    font-size: 16px;
    line-height: 24px;
  }

  &-slider {
    &__img {
      margin-bottom: 30px;
    }
  }
}

.blog {
  padding: 37px 0px 47px 0px;
  background-color: #f9f9f9;

  &__title {
    font-family: Roboto-Black;
    margin-bottom: 10px;
    font-size: 28px;
  }

  &__subtitle {
    font-family: Roboto-Bold;
    margin-bottom: 30px;
    font-size: 16px;
    color: #bf9d77;
  }

  &-article {
    padding: 20px;
    background-color: white;

    &__img {
      width: 100%;
    }

    &__title {
      font-family: Roboto-Bold;
      margin-bottom: 10px;
      font-size: 16px;
    }

    &__text {
      font-family: Roboto-Regular;
      margin-bottom: 20px;
      font-size: 12px;
      line-height: 18px;
    }
  }

  &-list {
    display: grid;
    gap: 20px;

    &__line {
      display: block;
      width: 100%;
      height: 1px;
      background-color: #bf9d77;
    }
  }

  &-item {
    display: grid;
    gap: 10px;

    &__title {
      font-family: Roboto-Bold;
      font-size: 16px;
      line-height: 24px;
    }
  }
}
</style>
