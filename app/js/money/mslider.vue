<template>
    <article>
        <Slider :items="items" :cname="$style.slider" />
        <section :class="$style.list">
            <router-link to="{name:'//sale.jd.com/m/act/ljXgxWmt0OVurynd.html?sid=&qingfrom=pcurl/?from=jrad_1830098'}">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t5842/235/8356236245/38364/2112fd7e/597a95d4Ne01da140.png?width=750&height=270" alt="">
            </router-link>
        </section>
    </article>
</template>

<script>
import Slider from '../core/slider.vue';
    export default {
        components:{
            Slider,
        },
        data(){
            return{
                items:[{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t11149/181/856008463/68797/dc303e9/59f97baeN3cdae084.jpg?width=750&height=400',
                    herf:'https://storage.jd.com/bk.jd.com/static/m/bcm_act.html?applyChannel=MOBILE-OPEN2&sid=&qingfrom=pcurl/?from=jrad_1830098'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t10405/120/2592801005/36022/d8f57852/59f97c14Nfb960073.png?width=750&height=400',
                    href:'home'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t9994/205/2575467053/189117/125e7b05/59f97c36N7599be57.png?width=750&height=400',
                    href:'home'
                }]
            }
        }
    }
</script>

<style lang="scss" module>
@import '../../css/element.scss';
.slider{
    margin:120px 0 20px;
    img{
        width:100%;
    }
}
section{
    background-color:#fff;
}
</style>