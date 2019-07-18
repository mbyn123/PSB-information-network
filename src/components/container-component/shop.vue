<template>
    <div>
        <Row>
            <Col span="16" offset="4">
                <div class="lists">
                    <div class="top" v-for="(value,index) in titles" :key="index">
                        <div class="titles">{{value.title}}</div>
                        <div class="tit">{{value.title2}}</div>
                        <div class="wire"></div>
                        <div class="gd"><img :src=value.img alt=""></div>
                    </div>
                </div>
            </Col>
        </Row>
        <Row>
            <Col span="16" offset="4">
                <div class="ww">
                    <Row>
                        <Col span="8" v-for="(value,index) in studys" :key="index">
                            <div class="alists">
                                <div class="top" >
                                    <div class="titles">{{value.title}}</div>
                                    <div class="wire"></div>
                                    <div style="margin-right:10px;padding-top: 10px "><img :src=value.img alt=""></div>
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
                        <Col span="8">
                            <div class="publicity">
                                <div style="position: relative" v-for="(value,index) in picture" :key="index">
                                    <img :src=value.img alt="">
                                </div>
                                <div>
                                    <Row>
                                        <Col :span=num(value) v-for="(value,index) in tabs" :key="index">
                                            <div class="lian">
                                                <div class="im" :style="{'background':color(value)}">
                                                    <Icon type="ios-create" size="40" class="ico"/>
                                                  {{value.tab}}
                                                </div>
                                            </div>
                                        </Col>
                                    </Row>
                                </div>
                            </div>
                        </Col>
                        <Col span="16">
                            <Row>
                                <div class="down">
                                <Col span="12" v-for="(value,index) in Document" :key="index">
                                    <div style="display: flex;">
                                        <div><a href=""><img :src=value.img alt="" style="width:100%;"></a></div>
                                        <div class="inner">
                                            <ul  class="conters">
                                                <li class="tit">{{value.Content}}</li>
                                                <li class="tit">{{value.Content2}}</li>
                                                <li class="tit">{{value.Content3}}</li>
                                                <li class="tit">{{value.Content4}}</li>
                                                <li class="tit">{{value.Content5}}</li>
                                            </ul>
                                        </div>
                                    </div>
                                </Col>
                                </div>
                            </Row>
                        </Col>
                    </Row>
                </div>
            </Col>
        </Row>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                titles:[
                    {
                        title:"交流园地",
                        title2:"/ IMAGES NEWS",
                        img:"http://ptt5and7y.bkt.clouddn.com/more.png"
                    }
                ],
                studys:[
                    {
                        title:"学习之窗",
                        img:"http://ptt5and7y.bkt.clouddn.com/more.png",
                        img2:require("../../assets/images/d1.png"),
                        title2: "乾县纪委深入贯彻十九大精神激发",
                        time2: "17-11-28",
                        title3: "乾县纪委创建“学习型廉洁型”机关",
                        time3: "17-11-27",
                        title4: "乾县纪委“四盏灯”照贫攻坚路",
                        time4: "17-11-26",
                        title5: "乾县纪委持续发力“四风”",
                        time5: "17-11-25",
                        title6: "乾县纪委“四个结贯彻十九大精神",
                        time6: "17-11-24",

                    },
                    {
                        title:"学习之窗",
                        img:"http://ptt5and7y.bkt.clouddn.com/more.png",
                        img2:require("../../assets/images/d1.png"),
                        title2: "乾县纪委深入贯彻十九大精神激发",
                        time2: "17-11-27",
                        title3: "乾县纪委创建“学习型廉洁型”机关",
                        time3: "17-11-26",
                        title4: "乾县纪委“四盏灯”照贫攻坚路",
                        time4: "17-11-25",
                        title5: "乾县纪委持续发力“四风”",
                        time5: "17-11-24",
                        title6: "乾县纪委“四个结贯彻十九大精神",
                        time6: "17-11-23",

                    },
                ],
                tabs: [
                    {
                        tab: "工作表格",
                    },
                    {
                        tab: "公车派遣",
                    },
                    {
                        tab: "学习园地",
                    },
                    {
                        tab: "数字证书",
                    },
                    {
                        tab: "通讯录",
                    },

                ],
                Document: [
                    {
                        img:require('../../assets/images/xzwd.jpg'),
                        Content: "乾县纪委深入贯彻十九大精神激发",
                        Content2: "乾县纪委创建“学习型廉洁型”机关",
                        Content3: "乾县纪委“四盏灯”照贫攻坚路",
                        Content4: "乾县纪委持续发力“四风”",
                        Content5: "乾县纪委“四个结贯彻十九大精神",
                    },
                    {
                        img:require('../../assets/images/xzrj.jpg'),
                        Content: "乾县纪委深入贯彻十九大精神激发",
                        Content2: "乾县纪委创建“学习型廉洁型”机关",
                        Content3: "乾县纪委“四盏灯”照贫攻坚路",
                        Content4: "乾县纪委持续发力“四风”",
                        Content5: "乾县纪委“四个结贯彻十九大精神",
                    },

                ],
                picture:[
                    {
                        img:require("../../assets/images/shipin.jpg")
                    }
                ]

            }
        },
        methods:{
            color(col){
                if(col.tab==="工作表格" ){
                    return "#308ccf"
                }else if(col.tab==="数字证书"){
                    return "#308ccf"
                }else {
                    return "#0e60b4"
                }
            },
            num(s){
                if(s.tab==="通讯录"){
                    return "24"
                }else{
                    return "12"
                }
            }
        }
    }
</script>

<style scoped>

    .down {
        border: 1px solid #ccc;
        margin-top: -175px;
        display: flex;
        margin-right: 10px;
        padding: 12px 0;
    }

    .down .inner {
        font-size: 14px;
        color: #333;
        padding: 10px;

    }

    .down .inner .conters .tit {
        margin-bottom: 5px;
        white-space:nowrap;
    }

    .down .inner .conters .tit:hover {
        cursor: pointer;
        color: #CBCBCB;
    }

    .publicity img {
        width: 100%;
        height: 218px
    }

    .publicity .lian {
        padding: 2px 0
    }

    .publicity .lian .ims {
        text-align: center;
        font-size: 20px;
        font-weight: bold;
        color: #fff;
        background: #0e60b4;
        margin-left: 7px;
        padding: 8px 0;
        cursor: pointer;
    }


    .publicity .lian .im {
        text-align: center;
        font-size: 20px;
        font-weight: bold;
        color: #fff;
        background: #0e60b4;
        margin:0 2px;
        padding: 8px 0;
        cursor: pointer;
    }

    .publicity .lian .im .ico {
        display: inline-block;
        vertical-align: top;
    }

    ul li {
        list-style: none;
    }

    .ww .alists .top .wire {
        display: inline-block;
        width: 50%;
        height: 1px;
        margin: auto 10px;
        background: #ccc;
    }

    .ww .alists .top {
        display: flex;
        justify-content: space-between;
    }

    .ww .alists .top .titles {
        background-color: #1258AE;
        height: 34px;
        line-height: 34px;
        text-align: center;
        color: #FFF;
        font-size: 20px;
        font-weight: bold;
        width:105px
    }


    .ww .lis {
        padding: 10px 10px 10px 0;

    }

    .ww .lis ul {
        border: 1px solid #ccc;
    }

    .ww .lis ul .wen {
        display: flex;
        justify-content: space-between;
        font-size: 14px;
        color: #333;
        padding: 10px 10px 5px 0;

    }

    .ww .lis ul .wen .cc:hover {
        color: #fff;
        cursor: pointer;
    }

    .ww .lis ul .wen img {
        margin: 0 10px;
    }

    .lists {

        margin-top: 10px;

    }

    .lists .top {
        display: flex;
        justify-content: space-between;
    }

    .lists .top .titles {
        padding: 5px 10px;
        font-size: 20px;
        font-weight: 600;
        color: #1258ae;
    }

    .lists .top .tit {
        font-size: 16px;
        font-weight: bold;
        color: #CBCBCB;
        margin: 0 60px;
        padding-top: 10px;
    }

    .lists .top .wire {
        display: inline-block;
        width: 50%;
        height: 1px;
        margin: auto 0;
        background: #ccc;
    }

    .lists .top .gd{
        padding-top: 10px;
    }
</style>