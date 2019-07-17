<template>
    <div>
        <div class="window">
            <Row>
                <Col span="8" >
                    <div class="lists">
                        <div class="top">
                            <div class="titles">学习之窗</div>
                            <div class="wire"></div>
                            <div style="margin-left:20px;padding-top: 10px "><img src="../../assets/images/more.png" alt=""></div>
                        </div>
                        <div class="lis">
                            <ul>
                                <li class="wen" v-for="(value,index) in windows" :key="index">
                                    <div>
                                    <img src="../../assets/images/d1.png" alt=""><span class="cc">{{value.title}}</span>
                                    </div>
                                    <div>
                                        <span>{{value.title2}}</span>
                                    </div>
                                </li>
                            </ul>
                        </div>
                    </div>
                </Col>
                <Col span="8" >
                    <div class="lists">
                        <div class="top">
                            <div class="titles">学习之窗</div>
                            <div class="wire"></div>
                            <div style="margin-left:20px;padding-top: 10px "><img src="../../assets/images/more.png" alt=""></div>
                        </div>
                        <div class="lis">
                            <ul>
                                <li class="wen" v-for="(value,index) in windows" :key="index">
                                    <div>
                                        <img src="../../assets/images/d1.png" alt=""><span class="cc">{{value.title}}</span>
                                    </div>
                                    <div>
                                        <span>{{value.title2}}</span>
                                    </div>
                                </li>
                            </ul>
                        </div>
                    </div>
                </Col>
                <Col span="8" >
                    <div class="lists">
                        <div class="top">
                            <div class="titles">学习之窗</div>
                            <div class="wire"></div>
                            <div style="margin-left:20px;padding-top: 10px "><img src="../../assets/images/more.png" alt=""></div>
                        </div>
                        <div class="lis">
                            <ul>
                                <li class="wen" v-for="(value,index) in windows" :key="index">
                                    <div>
                                        <img src="../../assets/images/d1.png" alt=""><span class="cc">{{value.title}}</span>
                                    </div>
                                    <div>
                                        <span>{{value.title2}}</span>
                                    </div>
                                </li>
                            </ul>
                        </div>
                    </div>
                </Col>
            </Row>
        </div>

    </div>

</template>

<script>
    export default {
        data(){
            return{
                windows:[
                    {
                        title:"乾县纪委深入贯彻十九大精神激发",
                        title2:"17-11-28",
                    },
                    {
                        title:"乾县纪委创建“学习型廉洁型”机关",
                        title2:"17-11-28",
                    },
                    {
                        title:"乾县纪委“四盏灯”照贫攻坚路",
                        title2:"17-11-28",
                    },
                    {
                        title:"乾县纪委持续发力“四风”",
                        title2:"17-11-28",
                    },
                    {
                        title:"乾县纪委“四个结贯彻十九大精神",
                        title2:"17-11-28",
                    },

                ]
            }
        }
    }
</script>

<style scoped>

    ul li{
        list-style: none;
    }

.window{
    width:1200px;
    margin: 0 auto;
    margin-top: 10px;
}

.window .lis{
    padding:10px 10px 10px 0;
}

    .window .lis ul{
        border:1px solid #ccc
    }

    .window .lis ul .wen {
        display: flex;
        justify-content: space-between;
        font-size: 14px;
        color: #333333;
        padding: 10px 10px 5px 0;
    }

    .window .lis ul .wen .cc:hover{
        color:#fff;
        cursor: pointer;
    }

    .window .lis ul .wen img{
        margin:0 10px;
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


.lists .top  .wire{
    display: inline-block;
    width:50%;
    height:1px;
    margin:auto  10px;
    background: #ccc;
}
</style>