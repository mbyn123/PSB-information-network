<template>
    <div>
        <div class="lists">
            <div class="top">
                <div class="titles">交流园地</div>
                <div class="tit">/ IMAGES NEWS</div>
                <div class="wire"></div>
                <div style="margin-left:195px;padding-top: 10px "><img src="../../assets/images/more.png" alt=""></div>
            </div>
        </div>
       <div class="ww">
           <Row>
               <Col span="8" >
                   <div class="alists">
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
                   <div class="alists">
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
               <Col span="8">
                   <div  class="publicity">
                       <div style="position: relative">
                           <img src="../../assets/images/shipin.jpg" alt="">
                       </div>
                       <div>
                           <Row>
                               <Col span="12">
                                <div class="lian" >
                                    <div class="im" style="background:#308ccf">
                                        <Icon type="ios-create" size="40" class="ico"/>  工作表格
                                    </div>
                                </div>
                               </Col>
                               <Col span="12">
                                   <div class="lian" >
                                       <div class="ims">
                                           <Icon type="ios-create" size="40" class="ico"/>  公车派遣
                                       </div>
                                   </div>
                               </Col>
                               <Col span="12">
                                   <div class="lian" >
                                       <div class="im">
                                           <Icon type="ios-create" size="40" class="ico"/>  学习园地
                                       </div>
                                   </div>
                               </Col>
                               <Col span="12" >
                                   <div class="lian" >
                                       <div class="ims" style="background:#308ccf">
                                           <Icon type="ios-create" size="40" class="ico"/>  数字证书
                                       </div>
                                   </div>
                               </Col>
                               <Col span="24">
                                   <div class="lian" >
                                       <div class="ims" style="margin: 0">
                                           <Icon type="ios-create" size="40" class="ico"/>  通讯录
                                       </div>
                                   </div>
                               </Col>
                           </Row>
                       </div>
                   </div>
               </Col>
               <Col span="16">
                   <div class="down" >
                       <div style="display: flex">
                           <div><a href=""><img src="../../assets/images/xzwd.jpg" alt=""></a></div>
                           <div class="aa">
                               <ul>
                                   <li>乾县纪委深入贯彻十九大精神激发</li>
                                   <li>乾县纪委创建“学习型廉洁型”机关</li>
                                   <li>乾县纪委“四盏灯”照贫攻坚路</li>
                                   <li>乾县纪委持续发力“四风”</li>
                                   <li>乾县纪委“四个结贯彻十九大精神</li>
                               </ul>
                           </div>
                       </div>
                       <div style="display: flex;margin-left: 50px">
                           <div><a href=""><img src="../../assets/images/xzrj.jpg" alt=""></a></div>
                           <div class="aa">
                               <ul>
                                   <li>乾县纪委深入贯彻十九大精神激发</li>
                                   <li>乾县纪委创建“学习型廉洁型”机关</li>
                                   <li>乾县纪委“四盏灯”照贫攻坚路</li>
                                   <li>乾县纪委持续发力“四风”</li>
                                   <li>乾县纪委“四个结贯彻十九大精神</li>
                               </ul>
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
        name: "Aside2",
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

.down{
    border:1px solid #ccc;
    margin-top: -180px;
    display: flex;
    margin-right: 10px;
    padding: 12px 0;
}

.down .aa{
    font-size: 14px;
    color:#333;
    padding: 10px ;

}

.down .aa ul li{
    margin-bottom: 5px;
}

.down .aa ul li:hover{
    cursor: pointer;
    color:#CBCBCB;
}

.publicity img{
    width: 100%;
    height:218px
}

.publicity .lian{
    padding:5px 0
}

.publicity .lian .ims{
    text-align: center;
    font-size: 20px;
    font-weight: bold;
    color: #fff;
    background: #0e60b4;
    margin-left:7px;
    padding: 8px 0;
    cursor: pointer;
}


.publicity .lian .im{
    text-align: center;
    font-size: 20px;
    font-weight: bold;
    color: #fff;
    background: #0e60b4;
    margin-right:7px;
    padding: 8px 0;
    cursor: pointer;
}

.publicity .lian .im .ico{
    display: inline-block;
    vert-align:top;
}

   ul li{
    list-style: none;
   }

  .ww .alists .top  .wire{
       display: inline-block;
       width:50%;
       height:1px;
       margin:auto  10px;
       background: #ccc;
   }

   .ww .alists .top{
       display: flex;
   }

   .ww .alists .top .titles{
       padding: 5px 10px;
       font-size: 20px;
       font-weight: 600;
       color:#fff;
       background: #1258ae;
   }

    .ww{
        width:1200px;
        margin: 0 auto;
    }

    .ww  .lis{
       padding:10px 10px 10px 0;

   }

   .ww .lis ul{
       border:1px solid #ccc
   }

   .ww .lis ul .wen {
       display: flex;
       justify-content: space-between;
       font-size: 14px;
       color: #333333;
       padding: 10px 10px 5px 0;
   }

   .ww .lis ul .wen .cc:hover{
       color:#fff;
       cursor: pointer;
   }

   .ww .lis ul .wen img{
       margin:0 10px;
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
        color:#1258ae;

    }

    .lists .top .tit{
        font-size:16px;
        font-weight: bold;
        color:#CBCBCB;
        margin: 0 60px;
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