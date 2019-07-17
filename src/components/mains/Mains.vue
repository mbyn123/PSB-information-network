<template>
    <div>
        <div style="border:1px solid red">
            111
            <slider :pages="pages" :sliderinit="sliderinit">
                <!-- slot  -->
            </slider>

        </div>
        <news/>
        <sections/>
        <list/>
        <sections2/>
        <lists/>
        <Asides/>
        <Aside2/>
        <figures/>
        <navigation/>
        <footers/>

    </div>
</template>

<script>
    import slider from 'vue-concise-slider'// 引入slider组件
    import news from "./news"
    import sections from "./sections"
    import List from "./List"
    import sections2 from "./sections2"
    import lists from "../component/lists"
    import Asides from "./Asides"
    import Aside2 from "./Aside2"
    import figures from "./figures"
    import navigation from "./navigation"
    import footers from "./footers"

    export default {
        data () {
            return {
                //图片列表[arr]
                pages:[
                    {
                        title: '',
                        style:{
                            background:'url(src/img/testimg-1.jpg)'
                        }
                    },
                    {
                        title: '',
                        style:{
                            background:'url(src/img/testimg-2.jpg)'
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
                    currentPage: 0,//当前页码
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
        components:{
            news,
            sections,
            List,
            sections2,
            lists,
            Asides,
            Aside2,
            figures,
            navigation,
            footers,
            slider
        }
    }
</script>

<style scoped>

</style>