<template>
    <div>
        <Row>
            <Col span="16" offset="4">
                <div class="lists">
                    <div class="top" v-for="(value ,index) in titles" :key="index">
                        <div class="titles">{{value.title}}</div>
                        <div class="tit">{{value.title2}}</div>
                        <div class="wire"></div>
                        <div class="gd"><img :src=value.img alt=""></div>
                    </div>
                </div>
                <Row>
                    <div class="picture">
                        <Col span="8" >
                            <div class="bigimg">
                                <a href="#" v-for="(value,index) in bigpictrues" :key="index">
                                    <img :src='value.img' alt="" style="height: 283px;width: 426px;">
                                    <div class="bgwz">{{value.title}}</div>
                                </a>
                            </div>
                        </Col>

                        <Col span="16">
                           <Row>
                               <Col span="6" v-for="(value ,index) in pictrues" :key="index">
                                   <div class="smimg" >
                                       <a href="#">
                                           <img :src="value.img" alt="">
                                           <div class="bgwz">{{value.title}}</div>
                                       </a>
                                   </div>
                               </Col>
                           </Row>
                        </Col>
                    </div>
                </Row>
            </Col>
        </Row>

    </div>
</template>
r
<script>
    export default {
        data() {
            return {
                titles: [
                    {
                        title: "本局风采",
                        title2: "/ The bureau elegant demeanour",
                        img: "http://ptt5and7y.bkt.clouddn.com/more.png"
                    }
                ],
                pictrues: [
                    {
                        title: "标题背景在图片上半透明",
                        img: "http://ptt5and7y.bkt.clouddn.com/2.jpg"
                    },
                    {
                        title: "标题背景在图片上半透明",
                        img: "http://ptt5and7y.bkt.clouddn.com/2.jpg"
                    },
                    {
                        title: "标题背景在图片上半透明",
                        img: "http://ptt5and7y.bkt.clouddn.com/2.jpg"
                    },
                    {
                        title: "标题背景在图片上半透明",
                        img: "http://ptt5and7y.bkt.clouddn.com/2.jpg"
                    },
                    {
                        title: "标题背景在图片上半透明",
                        img: "http://ptt5and7y.bkt.clouddn.com/2.jpg"
                    },
                    {
                        title: "标题背景在图片上半透明",
                        img: "http://ptt5and7y.bkt.clouddn.com/2.jpg"
                    },


                ],
                bigpictrues: [
                    {
                        title: "thinkcss标题背景在图片上半透明",
                        img: "http://ptt5and7y.bkt.clouddn.com/2.jpg"
                    },
                ]
            }
        }
    }
</script>

<style scoped>
    .picture {
        display: flex;
        margin-top: 10px;
    }

    .picture .bigimg {
        position: relative;
        overflow: hidden;
    }

    .picture .smimg .bgwz{
        font-size: 14px;
        font-weight: bold;
        color: #fff;
        background: rgba(0, 0, 0, .6);
        text-align: center;
        padding: 10px 0;
        position: absolute;
        bottom: 5px;
        width: 98%;
        height: 40px;
    }

    .picture .bigimg img {
        width: 100%;
        height: 100%;
        overflow: hidden;
    }

     .smimg {
        position: relative;
         width: 100%;
         height: 144px;
         padding: 2px;
         margin-left: 2px;

    }

   .smimg img {
        width: 100%;
        height: 100%;
    }

    .picture .smimg:hover .bgwz {
        height: 70px;
        background: rgba(0, 0, 0, .6);
    }


    .bigimg .bgwz {
        font-size: 14px;
        font-weight: bold;
        color: #fff;
        background: rgba(0, 0, 0, .6);
        text-align: center;
        padding: 10px 0;
        position: absolute;
        bottom: 5px;
        width: 100%;
        height: 40px;
    }

    .lists {

        margin-top: 10px;

    }

    .lists .top {
        display: flex;
        justify-content: space-between;
    }

    .lists .top .titles {
        background-color: #1258AE;
        height: 34px;
        line-height: 34px;
        text-align: center;
        color: #FFF;
        font-size: 20px;
        font-weight: bold;
        padding: 0 10px;
    }


    .lists .top .wire {
        width: 50%;
        height: 20px;
        border-bottom: 1px solid #ccc;;


    }

    .lists .top .gd {
        padding-top: 10px;
        margin-right: 10px;
    }

    .lists .top .tit {
        font-size: 16px;
        font-weight: bold;
        color: #CBCBCB;
        padding-top: 10px;

    }
</style>