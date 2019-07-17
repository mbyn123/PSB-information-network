<template>
    <div>
        <div class="message">
            <div class="f1"><img src="../../assets/images/gonggao.png" alt=""><span>泾阳召开 “ 六反十打 ” 第二战役总结暨第三战役动员会</span></div>
            <div class="f1"><img src="../../assets/images/zhiban.png" alt=""><span>局 领 导： 陈景锋 13892098188    法制大队： 罗建民 13619108966</span></div>
            <div class="mains">
                <div class="title">
                    <a href="#" title="习近平在全国网络安全和信息化工作会议上强调" style="font-size:16px">
                    <h1 >习近平在全国网络安全和信息化工作会议上强调</h1>
                   </a>
                </div>
                <div class="title2">
                    <span><a href="#">[我市17家重大火灾隐患单位被挂牌督办]</a> </span>
                    <span><a href="#">[广州市残联组织四场特殊教育学校开放日]</a> </span>
                    <span><a href="#">[集团年终贺岁晚会隆重举行 总裁期许集团明天更美好]</a></span>
                    <span><a href="#">[更多]</a></span>
                </div>
            </div>
        </div>
        <div class="side">
         <Row>
             <Col span="12">
                 <Carousel autoplay v-model="value2" loop   >
                     <CarouselItem>
                         <div class="demo-carousel">
                             <div style="position: relative">
                                 <div>
                                     <img src="../../assets/images/1.jpg" alt="">
                                     <div class="title3">
                                         <a href="#">泾阳召开“六反十打”第二战役总结暨第三战役动员会</a>
                                     </div>
                                 </div>
                             </div>
                         </div>
                     </CarouselItem>
                     <CarouselItem>
                         <div class="demo-carousel">
                             <div style="position: relative">
                                 <div>
                                     <img src="../../assets/images/2.jpg" alt="">
                                     <div class="title3">
                                         <a href="#">习近平：以永远在路上的执着把从严治党引向深入</a>
                                     </div>
                                 </div>
                             </div>
                         </div>
                     </CarouselItem>
                     <CarouselItem>
                         <div class="demo-carousel">
                             <div style="position: relative">
                                 <div>
                                     <img src="../../assets/images/1.jpg" alt="">
                                     <div class="title3">
                                         <a href="#">泾阳召开“六反十打”第二战役总结暨第三战役动员会</a>
                                     </div>
                                 </div>
                             </div>
                         </div>
                     </CarouselItem>
                     <CarouselItem>
                         <div class="demo-carousel">
                             <div style="position: relative">
                                 <div>
                                     <img src="../../assets/images/2.jpg" alt="">
                                     <div class="title3">
                                         <a href="#">习近平：以永远在路上的执着把从严治党引向深入</a>
                                     </div>
                                 </div>
                             </div>
                         </div>
                     </CarouselItem>

                 </Carousel>
             </Col>
             <Col span="12">
                 <div style="padding:20px;margin-left: 10px">
                      <div style="width:95%;padding-bottom:40px;border-bottom: 1px dotted #ccc">
                          <div>
                             <a href="#" style="color:#0071cf;font-size: 22px;font-weight: 600">泾阳召开“六反十打”第二战役总结暨第三战役动员会</a>
                          </div>
                          <div style="font-size: 14px;text-indent:2em">
                              6月5日，我县召开“六反十打”第二战役总结暨第三战役专项行动动员会，县委常委、常务副县长王敏，县委常委、宣传部部长张宣朝，县政府党组...
                              <span style="color:red;font-size: 10px">【2018-06-12】</span>
                          </div>
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
                    value2: 0
            }
        }
    }
</script>

<style scoped>

    .side{

        width:1200px;
        margin: 0 auto;
        margin-top: 10px;
    }
    .side .title3{
        position: absolute;
        bottom:0;
        background: rgba(0,0,0,0.6);
        padding: 10px;
        width:600px;
    }
    .side img{
        width:600px;
        height:406px;
    }
    .side .title3 a{
        color: #fff;
        font-size: 14px;
    }

    a{
        color:black
    }
.message{
    border-bottom:1px dotted #ccc;
    width:1200px;
    margin: 0 auto;
    padding:20px 0 ;
}
.message .f1{
    margin-left: 10px;
    display: inline-block;
    font-size: 14px;
    color:#333;
}
.message .f1 img{
    vertical-align: top;
    margin-right:10px ;
}
.message .title{
    text-align: center;
    margin-top: 38px;
}
    .message .title a{
      color:#0071cf
    }

.message .title2{
    text-align: center;
    margin: 12px 0;
}
    .message .title2 a{
        margin-right:5px;
    }
</style>