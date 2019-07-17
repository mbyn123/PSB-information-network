<template>
    <div >
       <div class="banner2" >
           <div >
               <img src="../../assets/images/banner1.jpg" alt="">
           </div>
       </div>
        <div class=" carousel2">
          <div ><img src="../../assets/images/zhuanti.jpg" alt=""></div>
            <div class="list">
              <div >
                 <div>
                     <slider :pages="pages" :sliderinit="sliderinit">

                     </slider>
                 </div>
              </div>
            </div>
        </div>
    </div>
</template>

<script>
    import slider from 'vue-concise-slider'// 引入slider组件
    export default {
        data () {
            return {
                //图片列表[arr]
                pages:[
                    {
                        title: '',
                        style:{
                            background:'url(../../assets/images/zhuanti.jpg)'
                        }
                    },
                    {
                        title: '',
                        style:{
                            background:'url(../../assets/images/zhuanti.jpg)'
                        }
                    },
                    {
                        title: 'slide3',
                        style:{
                            background:'#4bbfc3',
                        },
                    }
                ],
                //滑动配置[obj]
                sliderinit: {
                    currentPage: 1,//当前页码
                    thresholdDistance: 500,//滑动判定距离
                    thresholdTime: 100,//滑动判定时间
                    autoplay:1000,//自动滚动[ms]
                    loop:true,//循环滚动
                    direction:'vertical',//方向设置，垂直滚动
                    infinite:1,//无限滚动前后遍历数
                    slidesToScroll:1,//每次滑动项数
                }
            }
        },
        components: {
            slider
        }
    }
</script>

<style scoped>
.banner2{
    border:1px solid #ccc;
    width:1200px;
    margin: 0 auto;
    margin-top: 10px;
    padding:10px 10px 5px 10px;
}

.carousel2{
    border:1px solid red;
    width:1200px;
    margin: 0 auto;
    margin-top: 10px;
    display: flex;
}
.carousel2 .list{
    border:1px solid red;
}
</style>