<template>
    <div>
        <div class="footer" >
             <div v-for="(value,index) in footers" :key="index">{{value.title}}</div>
            <div style="margin-top: 20px">
                <a href="#" style="color:#939393;" v-for="(value,index) in Version" :key="index">
                    <img :src=value.img alt="">{{value.title}}
                </a>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data(){
            return{
                footers:[
                    {
                        title:"版权所有 @ 2016-2019 泾河新城公安分局 技术支持：美纳科技",
                    },
                    {
                        title:'联系电话：029-00000000 传真：029-00000000 地址：泾河新城 陕ICP备17020277号',
                    },
                ],

                Version:[
                    {
                        img:"http://ptt5and7y.bkt.clouddn.com/ga.png",
                        title:"陕公网安备 61042402000111号"
                    }
                ]
            }
        }
    }
</script>

<style scoped>
.footer{
    background-image: url(../assets/images/bg_foot.jpg);
    text-align: center;
    width:100%;
   font-size: 16px;
    padding:30px 0;
    margin-top: 20px;
}
    a{
        color: #333;
    }
</style>