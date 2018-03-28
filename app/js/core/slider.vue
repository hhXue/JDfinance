<template>
    <section :class="cname">
        <swiper :options="options">
            <swiper-slide v-for="item in items" :key="item.href">
                <img :src="item.src" alt=""/>
            </swiper-slide>
            <div class="swiper-pagination" slot="pagination"></div>
        </swiper>
    </section>
</template>

<script>
import { swiper, swiperSlide } from 'vue-awesome-swiper';
    export default {
        components: {
            swiper,
            swiperSlide
        },
        props:{
            cname:{
                type:String,
                default:''
            },
            options: {
                type:Object,
                default(){
                    return {
                        autoplay:true,
                        loop:true,
                        pagination:{
                            el: '.swiper-pagination',
                            clickable:true
                        },
                    }
                }
            },
            items:{
                type:Array,
                default(){
                    return []
                }
            },
        }
    }
</script>

<style lang="css">
@import '~swiper/dist/css/swiper.css';
</style>