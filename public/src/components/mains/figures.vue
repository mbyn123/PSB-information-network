<template>
    <div>
        <div class="lists">
            <div class="top">
                <div class="titles">本局风采</div>
                <div class="tit">/ The bureau elegant demeanou</div>
                <div class="wire"></div>
                <div style="margin-left:155px;padding-top: 10px "><img src="../../assets/images/more.png" alt=""></div>
            </div>
        </div>
        <div class="picture" >
            <div class="bgimg">
                <a href="#">
                    <img src="../../assets/images/2.jpg" alt="" style="height: 283px;width: 426px;">
                    <div class="bgwz">thinkcss标题背景在图片上半透明</div>
                </a>
            </div>
            <div style="display: flex;flex-wrap: wrap;">
                <div class="smimg" v-for="(value ,index) in pictrues" :key="index">
                    <a href="#">
                        <img src="../../assets/images/2.jpg" alt="">
                        <div class="bgwz">{{value.title}}</div>
                    </a>
                </div>
                </Row>
            </div>
        </div>
    </div>
</template>
r
<script>
    export default {
      data(){
          return{
            pictrues:[
                {
                    title:"标题背景在图片上半透明"
                },
                {
                    title:"标题背景在图片上半透明"
                },
                {
                    title:"标题背景在图片上半透明"
                },
                {
                    title:"文字背景在图片上半透明"
                },
                {
                    title:"文字背景在图片上半透明"
                },
                {
                    title:"文字背景在图片上半透明"
                },
                {
                    title:"文字背景在图片上半透明"
                },
            ]
          }
      }
    }
</script>

<style scoped>
    .picture{
        display: flex;
        margin: 10px auto;
        width:1200px;
    }

    .picture .bgimg{
        position: relative;
        margin-right: 2px;

    }

    .picture .smimg{
        height: 141px;
        width: 190px;
        position: relative;
        margin-right: 2px;

    }
    .picture .smimg img{
        width: 100%;
        height: 100%;
    }

    .picture .smimg:hover  .bgwz{
        height:70px;
        background: rgba(0,0,0,.6);
    }


    .picture .bgwz{
        font-size: 14px;
        font-weight: bold;
        color: white;
        background: rgba(0,0,0,.6);
        text-align: center;
        padding: 10px 0;
        position: absolute;
        bottom: 0;
        width: 100%;
        height: 40px;
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
        color:#fff;
        background: #1258ae;
    }

    .lists .top .tit{
        font-size:16px;
        font-weight: bold;
        color:#CBCBCB;
        margin: 0 20px;
        padding-top:10px;
    }
    .lists .top  .wire{
        display: inline-block;
        width:50%;
        height:1px;
        margin:auto  0;
        background: #ccc;
    }
</style>