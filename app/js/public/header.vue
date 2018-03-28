<template>
    <div :class="$style.header">
        <span>
            注册 | 登录
        </span>      
        <btn :class="$style.download">APP下载</btn>
    </div>
</template>

<script>
import btn from '../core/btn.vue'
    export default {
        components:{
            btn,
        }
    }
</script>

<style lang="scss" module>
.header{
    color:#666;
    height:100px;
    line-height:100px;
    position:fixed;
    top:0;
    left:0;
    right:0;
    z-index:100;
    background:#F9F9F9 url(//m.jr.jd.com/spe/qyy/main/images/jr-logo.png) center center no-repeat;
    background-size:auto 50%;
    span{
        font-size:28px;
        margin-left:24px;
    }
    .download{
        float:right;
        height:56px;
        line-height:56px;
        min-width:120px;
        margin:22px 24px 0 0;
    }
}
</style>