<template>
    <Panel title="理财精选" :class="$style.panel">
        <section :class="$style.content">
            <div :class="$style.item">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t3670/58/543125556/2606/a65096b9/580d80afN63b1085a.png?width=76&height=76" alt="">
                <div>
                    <h4>月度理财</h4>
                    <p>预期年化收益率4.50%</p>
                </div>
                <em>去赚钱<span> &gt;</span></em>
            </div>
            <div :class="$style.item">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t3679/44/511862277/2728/c1c6b2bf/580d8189N6b6f8052.png?width=76&height=76" alt="">
                <div>
                    <h4>季度理财</h4>
                    <p>预期年化收益率4.50%</p>
                </div>
                <em>去赚钱<span> &gt;</span></em>
            </div>
            <div :class="$style.item">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t3331/69/580199498/3074/d5bb21c5/580d7f6cN7f35e596.png?width=76&height=76" alt="">
                <div>
                    <h4>一年理财</h4>
                    <p>预期年化收益率4.50%</p>
                </div>
                <em>去赚钱<span> &gt;</span></em>
            </div>
        </section>
        
    </Panel>
</template>

<script>
import Panel from '../core/panel.vue';
    export default {
        components:{
            Panel,
        }
    }
</script>

<style lang="scss" module>
@import '../../css/element.scss';
.panel{
    @include panel;
    .content{
        @include flex;
        .item{
            @include flex(row);
            align-items:center;
            height:140px;
            img{
                width:88px;
                height:88px;
                margin:24px 32px 0;
            }
            >div{
                font-size:32px;
                color:#333;
                line-height:1.8;
                width:344px;
                white-space:nowrap;
                text-overflow:ellipsis;
                overflow:hidden;
                p{
                    font-size:24px;
                    color:#ff3232;
                    line-height:1.1;
                }
            }
            >em{
                font-size:28px;
                color:#FF801A;
                span{
                    color:#ccc;
                }
            }
        }
    }
  
}
</style>