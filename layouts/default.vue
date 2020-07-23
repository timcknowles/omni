<template>
  <div>
    <div>
      <topNav />
      <sideNav />
    </div>
  
    <div class="container is-widescreen">
      <nuxt />
    </div>
  </div>
</template>
<script>
import topNav from "~/components/navBar.vue";
import sideNav from "~/components/sideBar.vue";
export default {
  components: {
    topNav,
    sideNav

  }
};
</script>

<style lang="scss">
  @import '~assets/styles/main.scss';
</style>