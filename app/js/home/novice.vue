<template>

        <Panel :title="title"  :class="$style.panel">
            <section :class="$style.content">
                <div>
                    <h4>下载APP<span>送888元礼包</span></h4>
                    <p>新手专享</p>  
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t10384/155/1759179594/9776/185bd062/59e5f0ebNec4cf494.png?width=100&height=100" alt="">             
                </div>
                <div>
                    <ul>
                        <li>
                            <h4 :class="$style.redColor">领128元新手礼包</h4>
                            <p>立即开通</p>
                        </li>
                        <li>
                            <h4>打白条<span>享免息</span></h4>
                            <p>立即开通享豪礼</p>
                        </li>
                    </ul>
                </div>
            </section>
        </Panel>
  
</template>

<script>
import Panel from '../core/panel.vue';
    export default {
        components:{
            Panel,
        },
        data(){
            return{
                title:'新手特权'
            }
        }
    }
</script>

<style lang="scss" module>
@import '../../css/element.scss';
.grayColor{
    color:#999;
}
.redColor{
    color:#ff0000;
}
.panel{
    @include panel;
    >h4{
        border-bottom:1px solid #ddd;
    }
    .content{
        @include list(row);
        justify-content:space-around;
        color:#333;
        div{
            width:50%;
            &:first-child{
                background-size:132px auto;
                text-align:center;
                margin-bottom:28px;
            }
            img{
                width:132px;
                height:132px;
                margin-top:20px;
            }
            h4{
                font-size:26px;
                margin-top:32px;
                padding:0 108px 0 28px;
                line-height:40px;
                white-space:nowrap;
                text-overflow:ellipsis; 
                overflow:hidden;
            }
            >h4{
            padding:0 20px;
            }
            p{
                @extend .grayColor;
                font-size:24px;
                line-height:32px;
                margin:6px 0 0 0;
                padding:0 120px 34px 28px;
            }
            >p{
                padding:0;
            }
            li{
                border-left:1px solid #ddd;
                background:url(//img12.360buyimg.com/jrpmobile/jfs/t4804/179/657713323/5908/66dce262/58e6095fNd3dc3f39.png?width=100&height=100) right 28px center no-repeat;
                background-size:80px auto;
                h4{
                margin-top:0;
                padding-top:34px;
                }                                                                                              
                &:first-child{
                    background:url(//img12.360buyimg.com/jrpmobile/jfs/t4639/162/1782623297/60754/98ea03b4/58e60952N7fdb2b85.png?width=200&height=200) right 28px center no-repeat;
                    background-size:80px auto;
                    border-bottom:1px solid #ddd;
                    p{
                        margin-bottom:0;
                    }
                
                }
            }
            span{
                @extend .redColor;
            }
        }
    }

}
</style>