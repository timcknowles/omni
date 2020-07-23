<template>
    
  <vue-flip active-click width="200px" height="50px">
    <template v-slot:front class="front">
      front
    </template>
    <template v-slot:back class="back">
      back
    </template>

    
  </vue-flip>
  



</template>

<script>
import VueFlip from 'vue-flip';
export default {
  components: {
    'vue-flip': VueFlip
  }
}
</script>

<style>
  .front {
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #673AB7;
    color: white;
    width: 100%;
    height: 100%;
  }

  .back {
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #FFC107;
    color: white;
    width: 100%;
    height: 100%;
  }
</style>
