<template>
    <div>
        <div class="lists">
            <div class="top">
                <div class="titles">签收文件列表</div>
                <div class="tit">/ To sign for the file list</div>
                <div class="wire"></div>
                <div style="margin-left:155px;padding-top: 10px "><img src="../../assets/images/more.png" alt=""></div>
            </div>
            <div class="conter">
                <div class="ins">
                    <ul class="table">
                        <li class="tb1">文章标题</li>
                        <li class="tb2">发文单位</li>
                        <li class="tb3">需签单位</li>
                        <li class="tb4">发文时间</li>
                        <li class="tb5">签收状态</li>
                        <li class="tb6">签收情况</li>
                        <li class="tb7">签收</li>
                    </ul>
                     <ul class="table2" v-for="(value ,index) in tables" :key="index">
                         <li class="li1"><img :src=value.img alt=""></li>
                         <li class="li2">{{value.title1}}</li>
                         <li class="li3">{{value.title2}}</li>
                         <li class="li4">{{value.title3}}</li>
                         <li class="li5">{{value.title4}}</li>
                         <li class="li6">{{value.title5}}</li>
                         <li class="li7">{{value.title6}}</li>
                         <li class="li8"><a href="#"><img class="i"  :src=value.img2 alt="">{{value.title7}}</a></li>
                     </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data(){
            return{
                tables:[
                    {
                        img:'http://ptt5and7y.bkt.clouddn.com/txt.png',
                        title1:"关于开展互联网上网服务营业场所集中清查行动的通知",
                        title2:"网安大队",
                        title3:"查看",
                        title4:"2018年6月14",
                        title5:"签到中",
                        title6:"已签6单位",
                        img2:"http://ptt5and7y.bkt.clouddn.com/qstb.gif",
                        title7:'我要签到'
                    },
                    {
                        img:'http://ptt5and7y.bkt.clouddn.com/txt.png',
                        title1:"关于开展互联网上网服务营业场所集中清查行动的通知",
                        title2:"网安大队",
                        title3:"查看",
                        title4:"2018年6月14",
                        title5:"签到中",
                        title6:"已签6单位",
                        img2:"http://ptt5and7y.bkt.clouddn.com/qstb.gif",
                        title7:'我要签到'
                    },
                    {
                        img:'http://ptt5and7y.bkt.clouddn.com/txt.png',
                        title1:"关于开展互联网上网服务营业场所集中清查行动的通知",
                        title2:"网安大队",
                        title3:"查看",
                        title4:"2018年6月14",
                        title5:"签到中",
                        title6:"已签6单位",
                        img2:"http://ptt5and7y.bkt.clouddn.com/qstb.gif",
                        title7:'我要签到'
                    },
                    {
                        img:'http://ptt5and7y.bkt.clouddn.com/txt.png',
                        title1:"关于开展互联网上网服务营业场所集中清查行动的通知",
                        title2:"网安大队",
                        title3:"查看",
                        title4:"2018年6月14",
                        title5:"签到中",
                        title6:"已签6单位",
                        img2:"http://ptt5and7y.bkt.clouddn.com/qstb.gif",
                        title7:'我要签到'
                    },
                    {
                        img:'http://ptt5and7y.bkt.clouddn.com/txt.png',
                        title1:"关于开展互联网上网服务营业场所集中清查行动的通知",
                        title2:"网安大队",
                        title3:"查看",
                        title4:"2018年6月14",
                        title5:"签到中",
                        title6:"已签6单位",
                        img2:"http://ptt5and7y.bkt.clouddn.com/qstb.gif",
                        title7:'我要签到'
                    },
                ]
            }
        }
    }
</script>

<style scoped>
ul li{
    list-style: none;
}
a {
    color:#333
}
.lists .conter{
        border:1px solid #ccc;
        margin-top: 10px;
        padding: 10px 5px;
    }


.lists .conter .ins .table{
    display: flex;
    font-size: 14px;
    color:#333;
    text-align: center;
    background-color: #F8F8F8;
}

.lists .conter .ins .table2{
    display: flex;
    font-size: 14px;
    color:#333;
    text-align: center;
}

 .conter .ins .table  li{
    padding: 7px 0;
}

.conter .ins .table2  li{
    padding: 6px 0;
}

.lists .conter .ins .table .tb1{
    width:412px;
    border:1px solid #F3F3F3;
}

.lists .conter .ins .table .tb2{
    width:177px;
    border:1px solid #F3F3F3;
}

.lists .conter .ins .table .tb3{
    width:80px;
    border:1px solid #F3F3F3;
}

.lists .conter .ins .table .tb4{
    width:177px;
    border:1px solid #F3F3F3;
}

.lists .conter .ins .table .tb5{
    width:86px;
    border:1px solid #F3F3F3;
}

.lists .conter .ins .table .tb6{
    width:175px;
    border:1px solid #F3F3F3;
}

.lists .conter .ins .table .tb7 {
    width:119px;
    border:1px solid #F3F3F3;
}

.lists .conter .ins .table2 .li1{
    width:36px;
    border:1px solid #F3F3F3;
}

.lists .conter .ins .table2 .li2{
    width:362px;
    border:1px solid #F3F3F3;
}

.lists .conter .ins .table2 .li3{
    width:171px;
    border:1px solid #F3F3F3;
}

.lists .conter .ins .table2 .li4{
    width:78px;
    border:1px solid #F3F3F3;
}

.lists .conter .ins .table2 .li5{
    width:170px;
    border:1px solid #F3F3F3;
}

.lists .conter .ins .table2 .li6{
    width:84px;
    border:1px solid #F3F3F3;
}

.lists .conter .ins .table2 .li7{
    width:169px;
    border:1px solid #F3F3F3;
}

.lists .conter .ins .table2 .li8{
    width:115px;
    border:1px solid #F3F3F3;
}

.lists .conter .ins .table2 .li8 .i{
   display: inline-block;
    margin-top: 1px;
    vertical-align: top;

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
    color:#fff;
    background: #1258ae;
}

.lists .top .tit{
    font-size:16px;
    font-weight: bold;
    color:#CBCBCB;
    margin: 0 20px;
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