<template>
    <Panel title="新品推荐" :class="$style.panel">
        <section :class="$style.content">
            <div :class="$style.arrow">更多尖货 &gt;</div>
            <Slider :options="options" :items="items" cname="product-slider"/>        
        </section>
    </Panel>
</template>

<script>
import Panel from '../core/panel.vue';
import Slider from '../core/slider.vue';
    export default {
        components:{
            Panel,
            Slider,
        },
        data() {
            return {
                options: {
                    slidesPerView:2.2,
                    spaceBetween: 24,
                    freeMode: true
                },
                items:[{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t16591/349/2066779042/42386/92c7a2f6/5a7d5b56N263586c8.jpg?width=335&height=421',
                    href:'1'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t16858/332/448124625/49189/717a1c58/5a7d5b8cNa734cd9f.jpg?width=335&height=421',
                    href:'2'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t18736/21/452113740/50445/b97274fb/5a7d5bc4N592e324e.jpg?width=335&height=421',
                    href:'3'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t19438/256/457591773/38627/1f0fb065/5a7d5bd0N656c015c.jpg?width=335&height=421',
                    href:'4'
                }]
            }
        }
    }
</script>
<style lang="scss">
.product-slider {
    .swiper-container{
        padding:0 24px;
        .swiper-slide{
            img{
                width:100%;
                height:314px;
            }
        }
    }
}
</style>
<style lang="scss" module>
@import "../../css/element.scss";
.panel{
    @include panel;
    .content{
        position:relative;
        padding-bottom:24px;
        .arrow{
            position:absolute;
            top:-78px;
            right:32px;
            font-size:28px;
            color:#999;
        }
    }
}
</style>