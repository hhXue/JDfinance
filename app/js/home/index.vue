<template>
  <div>
      <Heador/>
      <Slider/>
      <Novice/>
      <Borrow/>
      <Money/>
      <Newproduct/>
      <Life/>
      <Help/>
      <Footor/>
      <Navbar/>
  </div>
</template>

<script>
import Heador from '../public/header.vue';
import Footor from '../public/footer.vue';
import Navbar from '../public/navbar.vue';
import Slider from './hslider.vue';
import Novice from './novice.vue';
import Borrow from './borrow.vue';
import Money from './money.vue';
import Newproduct from './newproduct.vue';
import Life from './life.vue';
import Help from './help.vue';


  export default {
    components:{
      Heador,
      Slider,
      Novice,
      Borrow,
      Money,
      Newproduct,
      Life,
      Help,
      Footor,
      Navbar,
    }
  }
</script>

<style lang="scss">
@import '../../css/reset.scss';
  
</style>