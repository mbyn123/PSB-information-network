<template>
    <div>
        <Row>
            <Col span="24" >
                <div class="banner">
                    <div class="topNav">
                        <div style="display: flex;justify-content: space-between;">
                        <div>
                            <span>欢迎光临泾河新城公安分局信息网!</span>
                            <span style="margin-left: 10px" e=""> 注册 | 登录</span>
                        </div>
                        <div class="nav">
                            <span><Icon class="ico" type="ios-phone-portrait" size="20"/>手机版</span>
                            <span><Icon class="ico" type="md-home" size="20"/>设为首页</span>
                            <span><Icon class="ico" type="ios-star" size="20"/>收藏本站</span>
                            <span><Icon class="ico" type="ios-pin" size="20"/>联系我们</span>
                        </div>
                        </div>
                    </div>
                    <div class="bgimg">
                        <div class="logo">
                            <a href="#">
                                <img src="../assets/images/logo.png" alt="">
                            </a>
                        </div>
                    </div>

                </div>
            </Col>
        </Row>
    </div>

</template>

<script>
    export default {
        name: "Head"
    }
</script>

<style scoped>
    .topNav{
        width: 1200px;
        margin: 0 auto;
        padding:7px 0;
        font-size: 14px;
        color:#333;
    }

    .topNav .nav span{
        margin-right: 30px;
    }

    .topNav .nav .ico{
        display: inline-block;
        vertical-align: top;
        margin-left: 5px;
    }
    .banner{
        height:293px;
        background-image: url(../assets/images/topbg.jpg);
    }

    .banner .bgimg{
        background-image: url(../assets/images/logobg.jpg);
        background-repeat: no-repeat;
        width:1200px;
        height:257px;
        margin: 0 auto;
    }
    .banner .logo{
        padding-top: 72px;

    }
</style>