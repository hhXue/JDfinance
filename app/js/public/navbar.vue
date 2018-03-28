<template>
    <Panel :class="$style.panel">
        <ul :class="$style.content">
            <li>
                <router-link :to="{name:'home'}">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t3451/188/644771475/2428/800d7cb7/580f2435Nbfaa8055.png?width=66&height=66" alt="">
                    <h4>首页</h4>
                </router-link>
            </li>
            <li>
                <router-link :to="{name:'money'}">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t3811/55/345433999/2930/116d3dd1/580f1e25N028a1f2c.png?width=66&height=66" alt="">
                    <h4>理财</h4>
                </router-link>
            </li>
            <li>
                <router-link :to="{name:'ious'}">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t3343/179/621044750/1484/5af6b11a/580f50e4N005181d0.png?width=66&height=66" alt="">
                    <h4>白条</h4>
                </router-link>
            </li>
            <li>
                <router-link :to="{name:'raise'}">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t3604/98/635506544/2317/443d3a51/580f240aNbee3dcc4.png?width=66&height=66" alt="">
                    <h4>众筹</h4>
                </router-link>
            </li>
            <li>
                <router-link :to="{name:'home'}">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t3340/68/639059082/2591/800e2d6b/580f51cdN4caf20b2.png?width=66&height=66" alt="">
                    <h4>我的</h4>
                </router-link>
            </li>
        </ul>
    </Panel>
</template>

<script>
import Panel from '../core/panel.vue';
    export default {
        components:{
            Panel,
        },
    }
</script>

<style lang="scss" module>
@import '../../css/element.scss';
.panel{
    @include panel;
    position:fixed;
    bottom:0;
    left:0;
    right:0;
    >h4{
        display:none;
    }
    .content{
        @include flex(row);
        justify-content:space-around;
        height:100px;
        li{
            a{
                text-decoration:none;
            }
            img{
                width:44px;
                height:44px;
                margin:12px auto 6px;
            }
            h4{
                font-size:22px;
                color:#656565;
            }
        }
    }
}
</style>