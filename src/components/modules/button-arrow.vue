<template>
  <div class="btn-arrow">
    <button class="btn-arrow__left">
      <img src="../../img/arrow-left-white.png" alt="err_img" />
    </button>
    <button class="btn-arrow__right">
      <img src="../../img/arrow-right-black.png" alt="err_img" />
    </button>
  </div>
</template>

<script></script>

<style scoped>
.btn-arrow {
  display: grid;
  width: 120px;
  height: 60px;
  grid-template-columns: repeat(2, 1fr);
}
.btn-arrow__left {
  width: 60px;
  height: 60px;
  align-items: center;
  justify-items: center;
  background-color: #bf9d77;
  color: #ffffff;
  border: 0px solid;
}
.btn-arrow__right {
  width: 60px;
  height: 60px;
  align-items: center;
  justify-items: center;
  background-color: #f9f9f9;
  color: #2b323c;
  border: 0px solid;
}
</style>
