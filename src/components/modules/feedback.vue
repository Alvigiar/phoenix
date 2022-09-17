<template>
  <section class="feedback">
    <div class="feedback__number">8 (812) 339-03-40</div>
    <img class="feedback__img-mail" src="../../img/mail.png" alt="err_img" />
    <span class="feedback__mail">info@npo-fenix.ru</span>
    <img class="feedback__img-time" src="../../img/time.png" alt="err_img" />
    <div class="feedback__work">
      <span class="feedback__chart">График работы:</span>
      <span class="feedback__time">пн-пт 08:00 - 16:45 (офис)</span>
    </div>
  </section>
</template>

<script></script>

<style scoped lang="scss">
.feedback {
  margin-bottom: 46px;
  display: grid;
  gap: 10px;
  grid-template-columns: 1em 10em;
  font-family: Roboto-Regular;
  font-size: 16px;
  &__number {
    grid-column: 1/4;
    font-family: Roboto-Black;
    font-size: 33px;
  }
  &__img-mail {
    align-self: center;
    grid-column: 1;
  }
  &__mail {
    grid-column: 2;
  }
  &__img-time {
    align-self: center;
    grid-column: 1;
  }
  &__work {
    grid-column: 2;
  }
}
</style>
