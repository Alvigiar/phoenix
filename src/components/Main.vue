<template>
  <section class="wrapper lab">
    <h1 class="lab__title">СОБСТВЕННАЯ ЛАБОРАТОРИЯ</h1>
    <div class="lab__text">
      ООО НПО "Феникс" обладает собственной, аккредитированной и сертифицированной
      лабораторией по определению химического состава черных и цветных металлов и их
      сплавов.
    </div>
    <button class="lab__details lab-details">
      <span class="lab-details__text">Подробнее</span>
      <div class="lab-details__cell">
        <img
          class="lab-details__arrow-img"
          src="../img/arrow-right-white.png"
          alt="err_img"
        />
      </div>
    </button>
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
        <div class="prod-box__line line-short"></div>
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
            <div class="services-box__line line-short"></div>
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
        <div class="blog-article__content">
          <h3 class="blog-article__title">Вторая жизнь металлолома</h3>
          <Article
            class="blog-article__img-info"
            dateText="20-10-2021"
            dateClock="08:10"
            viewNumb="30"
          />
          <div class="blog-_article_line line-short"></div>
          <div class="blog-article__text">
            Cдача металлолома позволяет многим организациям, не только навести порядок на
            своей территории, но и получить весомый доход.
          </div>
          <BtnDetails />
        </div>
      </article>
      <article class="blog__article blog-article">
        <img class="blog-article__img" src="../img/colormet.png" alt="err_img" />
        <div class="blog-article__content">
          <h3 class="blog-article__title">
            Цветной металлопрокат: особенности и разновидности
          </h3>
          <Article
            class="blog-article__img-info"
            dateText="12-10-2021"
            dateClock="10:13"
            viewNumb="34"
          />
          <div class="blog-_article_line line-short"></div>
          <div class="blog-article__text">
            Цветной металлопрокат применяют сегодня в машиностроении и электронике,
            военном производстве и строительстве, авиастроении и не только.
          </div>
          <BtnDetails />
        </div>
      </article>
      <Article
        title="Национальный сертификат лидера отрасли России"
        dateText="25-01-2021"
        dateClock="13:19"
        viewNumb="12"
      />
      <div class="blog-list__line line-long"></div>
      <Article
        title="Цветной металлопрокат: особенности и разновидности"
        dateText="25-03-2021"
        dateClock="14:22"
        viewNumb="18"
      />
      <div class="blog-list__line line-long"></div>
      <Article
        title="Вторая жизнь металлолома"
        dateText="25-05-2021"
        dateClock="17:56"
        viewNumb="15"
      />
      <div class="blog-list__line line-long"></div>
      <Article
        title="Национальный сертификат лидера отрасли России"
        dateText="25-01-2021"
        dateClock="13:19"
        viewNumb="12"
      />
    </div>
  </section>
</template>

<script>
import BtnArrow from "./modules/button-arrow.vue";
import BtnDetails from "./modules/button-detailed.vue";
import Article from "./modules/article.vue";

export default {
  name: "Main",
  components: {
    BtnArrow,
    BtnDetails,
    Article,
  },
};
</script>

<style scoped lang="scss">
.line {
  &-short {
    margin: 20px 0px;
    display: block;
    width: 55px;
    height: 1px;
    background-color: #bf9d77;
  }
  &-long {
    display: block;
    width: 100%;
    height: 1px;
    background-color: #bf9d77;
  }
}
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
  &-details {
    margin-bottom: 50px;
    display: flex;
    align-items: center;
    justify-content: center;
    border: 0 solid;
    font-family: Roboto;
    font-size: 16px;
    color: white;
    &__text {
      width: 150px;
      height: 60px;
      display: flex;
      align-items: center;
      justify-content: center;
      background-color: #983031;
    }
    &__cell {
      width: 60px;
      height: 60px;
      display: flex;
      align-items: center;
      justify-content: center;
      background-color: #983031;
      opacity: 0.9;
    }
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
  padding: 30px 0px 47px 0px;
  background-color: #f9f9f9;
  &-article {
    &__img {
      width: 100%;
      display: flex;
      &-info {
        padding: 0px;
      }
    }
    &__title {
      font-family: Roboto-Bold;
      font-size: 16px;
      line-height: 24px;
    }
    &__content {
      padding: 20px;
      margin-bottom: 15px;
      background-color: white;
    }
    &__text {
      margin-bottom: 20px;
      font-family: Roboto-Regular;
      font-size: 12px;
      line-height: 18px;
    }
  }
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

  &-list {
    display: grid;
    gap: 20px;
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
