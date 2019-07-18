<template>
    <div>

        <Row>
            <Col span="16" offset="4">
                <div class="banner2">
                    <div v-for="value in banner" :key="value.id">
                        <img :src=value.img alt="">
                    </div>
                </div>
            </Col>
        </Row>
        <Row>
            <Col span="16" offset="4">
                <Row>
                    <div class=" carousel2">
                    <Col span="2" v-for="value in titles" :key="value.id">
                        <div><img :src=value.img alt=""></div>
                    </Col>
                    <Col span="22">
                        <div class="list">
                            <div style="width:100%;position: relative">
                                <slider ref="slider" :options="options">
                                    <slideritem v-for="(item,index) in someList" :key="index" :style="item.style"
                                                style="width:500px">{{item.html}}
                                    </slideritem>
                                </slider>
                                <span class="btn1" @click=" slide "><Icon type="ios-arrow-back" size="30"/></span>
                                <span class="btn2" @click=" slideNext "><Icon type="ios-arrow-forward" size="30"/></span>
                            </div>
                        </div>
                    </Col>
                    </div>
                </Row>
            </Col>
        </Row>

    </div>
</template>

<script>
    import {slider, slideritem} from 'vue-concise-slider'

    export default {
        data() {
            return {
                titles:[
                    {
                        img:require("../assets/images/zhuanti.jpg")
                    }
                ],
                banner:[
                    {
                        img:require("../assets/images/banner1.jpg")
                    }
                ],
                someList: [

                    {
                        html: '',
                        style: {
                            'background': 'url("http://ptt5and7y.bkt.clouddn.com/z1.jpg") ',
                            'background-size': 'cover',
                            'width': '176px',
                            'height': '73px',
                            'margin-right': '2%',
                            'font-size': '30px',
                            'cursor': 'pointer'
                        }
                    },
                    {
                        html: '',
                        style: {
                            'background-image': 'url("http://ptt5and7y.bkt.clouddn.com/z2.jpg")',
                            'background-size': 'cover',
                            'width': '176px',
                            'height': '73px',
                            'margin-right': '1%',
                            'cursor': 'pointer'
                        }
                    },
                    {
                        html: '',
                        style: {
                            'background': 'url("http://ptt5and7y.bkt.clouddn.com/z1.jpg") ',
                            'background-size': 'cover',
                            'width': '176px',
                            'height': '73px',
                            'margin-right': '2%',
                            'font-size': '30px',
                            'cursor': 'pointer'
                        }
                    },
                    {
                        html: '',
                        style: {
                            'background-image': 'url("http://ptt5and7y.bkt.clouddn.com/z2.jpg")',
                            'background-size': 'cover',
                            'width': '176px',
                            'height': '73px',
                            'margin-right': '1%',
                            'cursor': 'pointer'
                        }
                    },
                    {
                        html: '',
                        style: {
                            'background': 'url("http://ptt5and7y.bkt.clouddn.com/z1.jpg") ',
                            'background-size': 'cover',
                            'width': '176px',
                            'height': '73px',
                            'margin-right': '2%',
                            'font-size': '30px',
                            'cursor': 'pointer'
                        }
                    },
                    {
                        html: '',
                        style: {
                            'background-image': 'url("http://ptt5and7y.bkt.clouddn.com/z2.jpg")',
                            'background-size': 'cover',
                            'width': '176px',
                            'height': '73px',
                            'margin-right': '1%',
                            'cursor': 'pointer'
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
                    autoplay: 3000,
                    speed: 600,
                    itemAnimation: true

                }
            }
        },
        components: {
            slider,
            slideritem
        },
        methods:{
            slideNext () {
                this.$refs.slider.$emit('slideNext')
            },
            slide () {
                this.$refs.slider.$emit('slidePre')
            }

        }
    }
</script>

<style scoped>

    .carousel2 .list .btn1{
          position: absolute;
          top:30%;
          left:-30px;
          cursor: pointer;
      }
    .carousel2 .list .btn2{
        position: absolute;
        top:30%;
        right:-30px;
        cursor: pointer;
    }
    .banner2 {
        border: 1px solid #ccc;
        margin-top: 10px;
        padding: 10px 10px 5px 10px;
    }

    .banner2 img {
        width: 100%;
    }

    .carousel2 {
        margin-top: 10px;
        display: flex;
    }

    .carousel2 .list {
        width: 100%;
        padding: 0 20px;
        margin-top: 10px;
    }
</style>
