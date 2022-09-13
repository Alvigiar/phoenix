<template>
  <Header />
  <Main />
  <Footer />
  <!-- <Slider /> -->
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Main from "./components/Main.vue";
// import Slider from "./components/modules/Slider.vue";

export default {
  name: "App",
  components: {
    Header,
    Footer,
    Main,
    // Slider,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
@media (min-width: 320px) {
  .wrapper {
    padding: 0px 20px;
  }
}

/* global style */

.slider-line {
  margin: 20px 0px;
  display: block;
  width: 55px;
  height: 1px;
  background-color: #bf9d77;
}
.btn__box-arrows {
  display: grid;
  width: 120px;
  height: 60px;
  grid-template-columns: repeat(2, 1fr);
}
.btn__arrow-left {
  width: 60px;
  height: 60px;
  align-items: center;
  justify-items: center;
  background-color: #bf9d77;
  color: #ffffff;
  border: 0px solid;
}
.btn__arrow-right {
  width: 60px;
  height: 60px;
  align-items: center;
  justify-items: center;
  background-color: #f9f9f9;
  color: #2b323c;
  border: 0px solid;
}
</style>
