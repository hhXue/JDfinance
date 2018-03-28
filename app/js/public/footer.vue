<template>
    <footer>
        <ul>
            <li>
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t2971/333/1297567079/898/f2d2e00d/577dc28dNe5138337.png?width=108&height=108" alt="">
                <h4>客户端</h4>
            </li>
            <li>
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t2824/256/2966087355/831/188bfa25/577cf3dcN18aadbf2.png?width=108&height=108" alt="">
                <h4>触屏版</h4>
            </li>
            <li>
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t2920/282/1283157010/1040/23f1430b/577cf3e5N53f740b8.png?width=108&height=108" alt="">
                <h4>电脑版</h4>
            </li>
        </ul>
        <p>Copyright &copy;2004-2018 京东JD.com 版权所有</p>
        <p>投资有风险，购买需谨慎</p>
        <p>京东金融平台服务协议</p>
        <p>京东金融隐私政策</p>
        
    </footer>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" module>
@import '../../css/element.scss';
footer{
    color:#999;
    font-size:26px;
    text-align:center;
    margin-bottom:120px;
    ul{
        @include flex(row);
        justify-content:space-around;
        padding-top:40px;
        margin-bottom:20px;
    }
    li{     
        h4{
            margin-top:12px;
        }
        img{
            width:90px;
            height:90px;
        }
    }
    p{
        font-size:24px;
        box-sizing:border-box;
        padding:24px 32px;
        border-top:1px solid #ddd;      
    }
}
</style>