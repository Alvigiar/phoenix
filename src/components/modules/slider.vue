<template>
  <div class="slider">
    <div class="slider-content">
      <div class="slider-title">{{ title }}</div>
      <div class="slider-line"></div>
      <div class="slider-subtitle">{{ subtitle }}</div>
    </div>
    <div class="slider-box__btn slider-btn">
      <button class="slider-btn__all">{{ btnBig }}</button>
      <div class="slider-btn__arrow slider-arrow">
        <button class="slider-arrow__left">{{ btnLeft }}</button>
        <button class="slider-arrow__right">{{ btnRight }}</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: "Title",
      subtitle: "Subtitle",
      btnBig: "One btn",
      btnLeft: "Left btn",
      btnRight: "Right btn",
    };
  },
};
</script>

<style scoped>
.slider {
  margin: 100px 50px;
}
.slider-content {
  padding: 190px 40px 0px 30px;
  display: block;
  background-color: burlywood;
}
.slider-title {
  font-weight: 700;
  font-size: 16px;
}
.slider-line {
  margin: 20px 0px;
  display: block;
  width: 55px;
  height: 1px;
  background-color: #bf9d77;
}
.slider-subtitle {
  padding-bottom: 30px;
  font-weight: 400;
  font-size: 16px;
}
.slider-box__btn {
  margin-top: 31px;
  height: 60px;
  display: grid;
  grid-template-columns: 150px 120px;
  gap: 11px;
}
.slider-btn__all {
  border: 0px solid;
  background-color: #bf9d77;
  color: white;
}
.slider-btn__arrow {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
}
.slider-arrow__left {
  border: 0px solid;
  background-color: #bf9d77;
  color: white;
}
.slider-arrow__right {
  border: 0px solid;
}
</style>
