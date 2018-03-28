<template>
    <Panel :class="$style.panel">
        <section :class="$style.content">
            <swiper :options="options">
                <swiper-slide>签到领流量，1元500M！</swiper-slide>
                <swiper-slide>百万白条劵，速来领取... <em>&gt;</em>  </swiper-slide>
            </swiper>
        </section>     
    </Panel>
</template>

<script>
import { swiper, swiperSlide } from 'vue-awesome-swiper';
import Panel from '../core/panel.vue';
    export default {
        components: {
            swiper,
            swiperSlide,
            Panel
        },
        data(){
            return{
                options: {
                    autoplay:true,
                    loop:true,
                    direction: 'vertical'
                }
            }
            
        }
    }
</script>
<style lang="scss">
.swiper-container{
    height:100%;
    .swiper-slide{
        em{
            color:#ddd;
            float:right;
            margin-right:20px;
        }
    }
}
</style>
<style lang="scss" module>
@import '../../css/element.scss';
.panel{
    @include panel;
    margin:120px 0 20px;
    >h4{
        display:none;
    }
    .content{
        height:72px;
        line-height:72px;
        overflow:hidden;
        font-size:28px;
        color:#333;
        padding-left:178px;
        background:url(//m.jr.jd.com/spe/qyy/main/images/scroll_title_img.png) left center no-repeat;
        
    }
}
</style>