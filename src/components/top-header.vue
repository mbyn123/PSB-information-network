<template>
    <div>
        <Row>
            <Col span="24" >
                <div class="banner">
                    <Row>
                        <Col span="16" offset="4">
                            <div class="topNav" v-for="(value,index) in register" :key="index">
                                <div style="display: flex;justify-content: space-between;">
                                    <div>
                                        <span class="text">{{value.title}}</span>
                                        <span  class="text" style="margin-left: 10px" > {{value.title2}}</span>
                                    </div>
                                    <div class="nav">
                                        <span class="links" v-for="value in links" :key="value.id">
                                            <Icon class="ico" :type=value.icon size="20"/>
                                            {{value.title}}
                                        </span>
                                    </div>
                                </div>
                            </div>
                        </Col>
                    </Row>
                    <Row>
                        <Col span="16" offset="4">
                             <div class="bigimg">
                        <div class="logo">
                            <a href="#">
                                <img src="../assets/images/logo.png" alt="">
                            </a>
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
                register:[
                    {
                        title:"欢迎光临泾河新城公安分局信息网!",
                        title2:"注册 | 登录",

                    }
                   ],
                links:[
                    {
                        title:"手机版",
                        icon:"ios-phone-portrait"

                    },
                    {
                        title:"设为首页",
                        icon:"md-home"

                    },
                    {
                        title:"收藏本站",
                        icon:"ios-star"

                    },
                    {
                        title:"联系我们",
                        icon:"ios-pin"
                    }
                ]
            }
        }
    }
</script>

<style scoped>
    .topNav{
        padding:7px 0;
        font-size: 14px;
        color:#333;
    }

    .topNav  .text{
        margin-right: 30px;
        cursor: pointer;
    }

    .topNav .nav .ico{
        display: inline-block;
        vertical-align: top;
        margin-left: 5px;
        cursor: pointer;
    }

    .topNav .nav .links{
        margin-left: 20px;
    }
    .banner{
        height:293px;
        background-image: url(../assets/images/topbg.jpg);
    }

    .banner .bigimg{
        background-image: url(../assets/images/logobg.jpg);
        background-repeat: no-repeat;

        height:257px;

    }
    .banner .logo{
        padding-top: 72px;

    }
</style>