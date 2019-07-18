<template>
    <div>
        <Row>
            <Col span="16" offset="4">
                <div class="bgnav" v-for="value in titles" :key="value.id">
                    <div><img :src=value.img alt="" style="width:100%;height:100%"></div>
                    <div class="in">
                        <ul class="aniu">
                            <li v-for="(value,index) in anius" :key="index">
                                <a href="#">
                                    <img :src=value.img alt="" style="width:100%">
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </Col>
        </Row>
        <Row>
            <Col span="16" offset="4">
                <div class="lists">
                    <div class="top" v-for="(value,index) in navs" :key="index">
                        <div class="titles">{{value.title}}</div>
                        <div class="tit">{{value.title2}}</div>
                        <div class="wire"></div>
                        <div class="link" >
                            <span v-for="(value,index) in items" :key="index">{{value.title}}</span>
                        </div>
                    </div>
                </div>
            </Col>
        </Row>
        <Row>
            <Col span="16" offset="4">


                     <div style="width:100%;">
                         <!-- Using the slider component -->
                         <slider ref="slider" :options="options" >
                             <!-- slideritem wrapped package with the components you need -->
                             <slideritem v-for="(item,index) in someList" :key="index" :style="item.style" style="width:500px">{{item.html}}</slideritem>

                             <!-- Customizable loading -->

                         </slider>
                     </div>

            </Col>
        </Row>
    </div>
</template>

<script>
    import { slider, slideritem } from 'vue-concise-slider'
    export default {
        data() {
            return {
                titles:[
                    {
                        img:require("../../assets/images/bgan.jpg")
                    }
                ],
                navs: [
                    {
                        title: "视频中心",
                        title2: "/ video",
                        title4: "公益广告",
                    }
                   ],
                items:[
                    {
                        title: "动漫",
                    },
                    {
                        title: "公益广告",
                    },
                    {
                        title:  "微电影",
                    },
                    {
                        title: "镜头",
                    },
                    {
                        title:  "图解",
                    },
                ],
                anius:[
                    {
                        img:"http://ptt5and7y.bkt.clouddn.com/bg1.jpg",
                    },
                    {
                        img:"http://ptt5and7y.bkt.clouddn.com/bg2.jpg",
                    },
                    {
                        img:"http://ptt5and7y.bkt.clouddn.com/bg3.jpg",
                    },
                    {
                        img:"http://ptt5and7y.bkt.clouddn.com/bg4.jpg",
                    },
                    {
                        img:"http://ptt5and7y.bkt.clouddn.com/bg5.jpg",
                    },
                    {
                        img:"http://ptt5and7y.bkt.clouddn.com/bg6.jpg",
                    }
                ],
                someList : [

                    {
                        html: '',
                        style: {
                            'background': 'url("http://ptt5and7y.bkt.clouddn.com/1.jpg") ',
                            'background-size': 'cover',
                            'width': '266px',
                            'height': '166px',
                            'margin-right': '2%',
                            'font-size':'30px',

                        }
                    },
                    {
                        html: '',
                        style: {
                            'background-image': 'url("http://ptt5and7y.bkt.clouddn.com/1.jpg")',
                            'background-size': 'cover',
                            'width': '266px',
                            'height': '166px',
                            'margin-right': '1%',

                        }
                    },
                    {
                        html: '',
                        style: {
                            'background-image': 'url("http://ptt5and7y.bkt.clouddn.com/1.jpg")',
                            'background-size': 'cover',
                            'width': '266px',
                            'height': '166px',
                            'margin-right': '1%',

                        }
                    },
                    {
                        html: '',
                        style: {
                            'background-image': 'url("http://ptt5and7y.bkt.clouddn.com/1.jpg")',
                            'background-size': 'cover',
                            'width': '266px',
                            'height': '166px',
                            'margin-right': '1%',

                        }
                    },
                    {
                        html: '',
                        style: {
                            'background-image': 'url("http://ptt5and7y.bkt.clouddn.com/1.jpg")',
                            'background-size': 'cover',
                            'width': '266px',
                            'height': '166px',
                            'margin-right': '1%',

                        }
                    },
                    {
                        html: '',
                        style: {
                            'background-image': 'url("http://ptt5and7y.bkt.clouddn.com/1.jpg")',
                            'background-size': 'cover',
                            'width': '266px',
                            'height': '166px',
                            'margin-right': '1%',

                        }
                    },


                ],
                options: {
                    currentPage: 0,
                   tracking: false,
                    thresholdDistance: 10,
                 //   thresholdTime: 3000,
                  //  infinite: 4,
                    slidesToScroll: 1,
                    loop: true,
                    autoplay: 1000,
                    speed: 600,
                    itemAnimation: true
                }
            }
        },
        components: {
            slider,
            slideritem
        }


    }
</script>

<style scoped>
    ul li {
        list-style: none;

    }

    .bgnav {

        border: 1px solid #ccc;
        display: flex;
        justify-content: space-between;
        margin-top: 10px;
    }
    .bgnav .in{
        padding:20px
    }

    .bgnav .in .aniu {
        display: flex;
    }

    .bgnav .in .aniu li {
      margin-left: 20px;
    }

    .lists {

        margin-top: 10px;

    }

    .lists .top{
        display: flex;
        justify-content: space-between;
    }
    .lists .top .titles{

        height: 34px;
        line-height: 34px;
        text-align: center;
        color: #333;
        font-size: 20px;
        font-weight: bold;
        padding: 0 10px;
    }


    .lists .top  .wire{
        width:50%;
        height:20px ;
        border-bottom:1px solid #ccc;;
    }


    .lists .top .tit{
        font-size:16px;
        font-weight: bold;
        color:#CBCBCB;
        padding-top:5px;


    }

    .lists .top .link span {
        font-size: 14px;
        margin-left: 10px;
        cursor: pointer;
    }

    .lists .top .link span:hover {
        color: #fff
    }
</style>