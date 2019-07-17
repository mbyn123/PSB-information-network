<template>
    <div>
        <div class="bgnav">
            <div><img src="../../assets/images/bgan.jpg" alt=""></div>
            <div class="in">
                <ul class="aniu">
                    <li><a href="#"><img src="../../assets/images/bg1.jpg" alt=""></a></li>
                    <li><a href="#"><img src="../../assets/images/bg2.jpg" alt=""></a></li>
                    <li><a href="#"><img src="../../assets/images/bg3.jpg" alt=""></a></li>
                    <li><a href="#"><img src="../../assets/images/bg4.jpg" alt=""></a></li>
                    <li><a href="#"><img src="../../assets/images/bg5.jpg" alt=""></a></li>
                    <li><a href="#"><img src="../../assets/images/bg6.jpg" alt=""></a></li>

                </ul>
            </div>
        </div>
        <div class="lists">
            <div class="top">
                <div class="titles">视频中心</div>
                <div class="tit">/ video</div>
                <div class="wire"></div>
                <div class="link">
                    <span>动漫</span>
                    <span>公益广告</span>
                    <span>微电影</span>
                    <span>镜头</span>
                    <span>图解</span>
                </div>
            </div>
        </div>
        <div style="width:1200px;height:200px;border:1px solid red;margin: 0 auto">

        </div>


    </div>
</template>

<script>

    export default {


    }
</script>

<style scoped>
    ul li{
        list-style: none;
    }

.bgnav{
    width:1200px;
    margin: 10px auto;
    border:1px solid #ccc;;
    display: flex;
    }


    .bgnav .in .aniu{
        display: flex;
       padding-top:25px ;

    }
    .bgnav .in .aniu li{
          margin-left: 20px;
    }

    .lists{
        margin: 0 auto;
        width:1200px;
        margin-top: 10px;

    }
    .lists .top{
        display: flex;
    }
    .lists .top .titles{
        padding: 5px 10px;
        font-size: 20px;
        font-weight: 600;
        color: #0e60b4;

    }

    .lists .top .tit{
        font-size:16px;
        font-weight: bold;
        color:#CBCBCB;
        margin: 0 30px;
        padding-top:10px;
    }
    .lists .top  .wire{
        display: inline-block;
        width:50%;
        height:1px;
        margin:auto  0;
        background: #ccc;
    }
    .lists .top .link{
        margin-left:155px;
        padding-top: 10px;
    }
    .lists .top .link span{
        font-size: 14px;
        margin-left: 10px;
        cursor: pointer;
    }

    .lists .top .link span:hover{
        color:#fff
    }
</style>