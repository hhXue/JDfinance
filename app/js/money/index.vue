<template>
  <div>
      <Heador/>
      <Slider/>
      <Recommend/>
      <Ad/>
      <Money/>
      <Adb/>
      <Footor/>
      <Navbar/>
  </div>
</template>

<script>
import Heador from '../public/header.vue';
import Footor from '../public/footer.vue';
import Navbar from '../public/navbar.vue';
import Slider from './mslider.vue';
import Recommend from './recommend.vue';
import Ad from './ad.vue';
import Money from './money.vue';
import Adb from './adb.vue';
  export default {
    components:{
      Heador,
      Slider,
      Footor,
      Navbar,
      Recommend,
      Ad,
      Money,
      Adb,
    }
  }
</script>

<style lang="scss">
@import '../../css/reset.scss';
  
</style>