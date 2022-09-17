<template>
  <button class="btn-details">
    <span class="btn-details__text">Подробнее</span>
    <div class="btn-details__cell">
      <img
        class="btn-details__arrow-img"
        src="../../img/arrow-detail.png"
        alt="err_img"
      />
    </div>
  </button>
</template>

<script>
export default {
  props: {
    isLabBox: {
      type: Boolean,
      default: false,
    },
  },
};
</script>

<style scoped lang="scss">
.btn {
  &-details {
    display: flex;
    align-items: center;
    height: 18px;
    border: 0px solid;
    color: #bf9d77;
    background-color: white;
    &__text {
      margin-right: 10px;
      font-family: Roboto-Regular;
      font-size: 12px;
    }
  }
}
</style>
