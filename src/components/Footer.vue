<template>
  <footer class="wrapper footer">
    <Logo/>
  </footer>
</template>

<script>
import Logo from "./modules/logo.vue";

export default {
  components: {
    Logo,
  }
};
</script>

<style scoped lang="scss">
.footer {
  &__title {
    width: 100%;
  }
}
</style>
