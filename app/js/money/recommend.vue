<template>
    <Panel title="精选推荐" :class="$style.panel">
        <section :class="$style.content">
            <dl :class="$style.item" v-for="item in items" :key="item.title">
                <dt><label>{{item.title}}</label><span>{{item.sub}}</span></dt>
                <dd>{{item.ratel}}</dd>
                <dd>{{item.text}}</dd>
            </dl>
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
                items:[{
                    title:'定期理财',
                    sub:'90天可质押',
                    ratel:'5.50%',
                    text:'历史年化结算利率'
                },
                {
                    title:'固收理财',
                    sub:'理财首选',
                    ratel:'5.80%',
                    text:'综合年化收益率'
                },
                {
                    title:'基智账户',
                    sub:'组合投资',
                    ratel:'8%-10%',
                    text:'止盈年化收益率'
                },
                {
                    title:'小白基金',
                    sub:'天天赚钱',
                    ratel:'4.27%',
                    text:'7日年化收益率'
                }]
            }
        }
    }
</script>

<style lang="scss" module>
@import '../../css/element.scss';
.panel{
    @include panel;
    .content{
        @include flex(row);
        .item{
            box-sizing:border-box;
            width:50%;
            height:218px;
            padding-left:32px;
            font-family: PingFangSC-Medium;
            dt{
                color: #333;
                font-weight: 700;
                font-size: 30px;
                display: block;
                height: 42px;
                line-height: 42px;
                box-sizing: border-box;
                margin: 34px 0 16px;
                white-space: nowrap;
                text-overflow: ellipsis;
                overflow: hidden;
                label{
                    float:left;
                    font-weight:700
                }
                span{
                    height: 34px;
                    line-height: 34px;
                    font-size: 22px;
                    padding: 0 4px;
                    color: #FF5155;
                    position: relative;
                    top: 3px;
                    left: 8px;
                    text-align: center;
                    float: left;
                    border:1px solid red;
                }
            }
            dd{
                &:nth-child(2){
                    font-weight: 700;
                    font-size: 44px;
                    height: 58px;
                    line-height: 58px;
                    color: #FF5155;
                    white-space: nowrap;
                    text-overflow: ellipsis;
                    overflow: hidden;
                }
                &:nth-child(3){
                    font-size: 24px;
                    height: 34px;
                    line-height: 34px;
                    color: #999;
                    white-space: nowrap;
                    text-overflow: ellipsis;
                    overflow: hidden;
                }
            }
        }
    }
}
</style>