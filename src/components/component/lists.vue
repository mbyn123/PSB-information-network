<template>
    <div>
        <Row>
            <Col span="16" offset="4">
               <div class="window">
            <Row>
                <Col span="8" v-for="(value,index) in files" :key="index">
                    <div class="lists">
                        <div class="top">
                            <div class="titles"><span>{{value.title}}</span></div>
                            <div class="wire"></div>
                            <span class="gd"><img :src=value.img alt=""></span>
                        </div>
                        <div class="lis">
                            <ul>
                                <li class="wen" >
                                    <div>
                                    <img :src=value.img2 alt=""><span class="cc">{{value.title2}}</span>
                                    </div>
                                    <div>
                                        <span>{{value.time2}}</span>
                                    </div>
                                </li>
                                <li class="wen" >
                                    <div>
                                        <img :src=value.img2 alt=""><span class="cc">{{value.title3}}</span>
                                    </div>
                                    <div>
                                        <span>{{value.time3}}</span>
                                    </div>
                                </li>
                                <li class="wen" >
                                    <div>
                                        <img :src=value.img2 alt=""><span class="cc">{{value.title4}}</span>
                                    </div>
                                    <div>
                                        <span>{{value.time4}}</span>
                                    </div>
                                </li>
                                <li class="wen" >
                                    <div>
                                        <img :src=value.img2 alt=""><span class="cc">{{value.title5}}</span>
                                    </div>
                                    <div>
                                        <span>{{value.time5}}</span>
                                    </div>
                                </li>
                                <li class="wen" >
                                    <div>
                                        <img :src=value.img2 alt=""><span class="cc">{{value.title6}}</span>
                                    </div>
                                    <div>
                                        <span>{{value.time6}}</span>
                                    </div>
                                </li>
                            </ul>
                        </div>
                    </div>
                </Col>
            </Row>
        </div>
            </Col>
        </Row>
    </div>

</template>

<script>
    export default {
        data(){
            return{
                files:[
                    {
                        title:"学习之窗",
                        img:require("../../assets/images/more.png"),
                        img2:require('../../assets/images/d1.png'),
                        title2:"乾县纪委深入贯彻十九大精神激发",
                        time2:"17-11-28",
                        title3:"乾县纪委创建“学习型廉洁型”机关",
                        time3:"17-11-27",
                        title4:"乾县纪委“四盏灯”照贫攻坚路",
                        time4:"17-11-26",
                        title5:"乾县纪委持续发力“四风”",
                        time5:"17-11-25",
                        title6:"乾县纪委“四个结贯彻十九大精神",
                        time6:"17-11-24",
                    },
                    {
                        title:"学习之窗",
                        img:require("../../assets/images/more.png"),
                        img2:require('../../assets/images/d1.png'),
                        title2:"乾县纪委深入贯彻十九大精神激发",
                        time2:"17-11-28",
                        title3:"乾县纪委创建“学习型廉洁型”机关",
                        time3:"17-11-27",
                        title4:"乾县纪委“四盏灯”照贫攻坚路",
                        time4:"17-11-26",
                        title5:"乾县纪委持续发力“四风”",
                        time5:"17-11-25",
                        title6:"乾县纪委“四个结贯彻十九大精神",
                        time6:"17-11-24",
                    },
                    {
                        title:"学习之窗",
                        img:require("../../assets/images/more.png"),
                        img2:require('../../assets/images/d1.png'),
                        title2:"乾县纪委深入贯彻十九大精神激发",
                        time2:"17-11-28",
                        title3:"乾县纪委创建“学习型廉洁型”机关",
                        time3:"17-11-27",
                        title4:"乾县纪委“四盏灯”照贫攻坚路",
                        time4:"17-11-26",
                        title5:"乾县纪委持续发力“四风”",
                        time5:"17-11-25",
                        title6:"乾县纪委“四个结贯彻十九大精神",
                        time6:"17-11-24",
                    },


                ],
            }
        }
    }
</script>

<style scoped>

    ul li{
        list-style: none;
    }

.window{

    margin-top: 10px;
}

.window .lis{
    padding:10px 10px 10px 0;
}



    .window .lis  .wen {
        display: flex;
        justify-content: space-between;
        font-size: 14px;
        color: #333333;
        padding: 10px 10px 5px 0;
    }

    .window .lis  .wen .cc:hover{
        color:#fff;
        cursor: pointer;
    }

    .window .lis  .wen img{
        margin:0 10px;
    }

.lists .top{
      display: flex;
    justify-content: space-between;
}
.lists .top .titles{
    background-color: #1258AE;
    height: 34px;
    line-height: 34px;
    text-align: center;
    color: #FFF;
    font-size: 20px;
    font-weight: bold;
    padding: 0 10px;
}


.lists .top  .wire{
     width:50%;
     height:20px ;
     border-bottom:1px solid #ccc

}
    .lists .top .gd{
        padding-top: 10px;
        margin-right: 10px;
    }
</style>