<template>
  <div>
    <div>
      <Nav />
    </div>
  
    <div class="container is-widescreen">
      <nuxt />
    </div>
  </div>
</template>
<script>
import Nav from "~/components/navBar.vue";
export default {
  components: {
    Nav
  }
};
</script>

<style lang="scss">
  @import '~assets/styles/main.scss';
</style>