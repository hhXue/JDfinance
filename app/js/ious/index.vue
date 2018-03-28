<template>
  <div>
      <Heador/>
      <Slider/>
      <Welfare/>
      <More/>
      <Help/>
      <Footor/>
      <Navbar/>
  </div>
</template>

<script>
import Heador from '../public/header.vue';
import Footor from '../public/footer.vue';
import Navbar from '../public/navbar.vue';
import Slider from './islider.vue';
import Welfare from './welfare.vue';
import More from './more.vue';
import Help from './help.vue';
  export default {
    components:{
      Heador,
      Slider,
      Welfare,
      More,
      Help,
      Footor,
      Navbar,
    }
  }
</script>

<style lang="scss">
@import '../../css/reset.scss';
  
</style>