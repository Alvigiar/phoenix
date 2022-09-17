<template>
  <article class="article">
    <h3 class="article__title">{{ title }}</h3>
    <div class="info">
      <div class="info-date">
        <img class="info-date__img" src="../../img/calendar.png" alt="err_img" />
        <span class="info-date__text">{{ dateText }}, {{ dateClock }}</span>
      </div>
      <div class="info-view">
        <img class="info-view__img" src="../../img/eye.png" alt="err_img" />
        <span class="info-view__numb">{{ viewNumb }}</span>
      </div>
    </div>
  </article>
</template>

<script>
export default {
  props: {
    title: String,
    dateText: String,
    dateClock: Number,
    viewNumb: Number,
  },
};
</script>

<style scoped lang="scss">
.article {
  padding: 17px;
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
.info {
  display: flex;
  &-date {
    &__text {
      margin: 0px 30px 0px 10px;
      font-family: Roboto-Regular;
      font-size: 12px;
      color: #2b323c;
      opacity: 0.4;
    }
  }
  &-view {
    &__numb {
      margin-left: 10px;
      font-family: Roboto-Regular;
      font-size: 12px;
      color: #2b323c;
      opacity: 0.4;
    }
  }
}
</style>
