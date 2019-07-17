<template>
    <div>
        <div class="navigate">
            <ul class="in" >
                <li><a href="#"><Icon type="ios-home-outline" class="ii"/><span>网站首页</span></a></li>
                <li><a href="#"><Icon type="ios-card-outline" class="ii"/><span>机构设置</span></a></li>
                <li><a href="#"><Icon type="md-book" class="ii"/><span>分局概况</span></a></li>
                <li><a href="#"><Icon type="md-heart-outline" class="ii"/><span>分局文件</span></a></li>
                <li><a href="#"><Icon type="ios-list" class="ii"/><span>巡视巡察</span></a></li>
                <li><a href="#"><Icon type="ios-hammer-outline" class="ii"/><span>图片视频</span></a></li>
                <li><a href="#"><Icon type="ios-leaf-outline" class="ii" /><span>业务之窗</span></a></li>
                <li><a href="#"><Icon type="ios-image-outline" class="ii"/><span>工作动态</span></a></li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: "nav.vue"
    }
</script>

<style scoped>
    a{
        color:black
    }
    ul li{
        list-style: none;
    }
.navigate{
    width:1200px;
    margin: 0 auto;
    background: #0071cf;
    height: 60px;
    line-height: 60px;

}
    .navigate .in{
       display: flex;
        justify-content: space-evenly;

    }
    .navigate .in a{
        display: block;
        color:white;
        font-size: 18px;
        font-weight: 600;

    }
    .navigate .in a span:hover{
        color:red
    }
    .navigate .in a .ii{
        font-size:30px;
        display: inline-block;
        vertical-align: middle;
        margin-right: 5px;
    }
</style>