<template>
    <div>
        <Row>
            <Col span="16" offset="4">
               <div class="navigate">
            <ul class="in" >
                <li v-for="(value,index) in shop" :key="index">
                    <a href="#"><Icon :type=value.icon class="ii"/>
                        <span>{{value.title}}</span>
                    </a>
                </li>
            </ul>
        </div>
            </Col>
        </Row>
    </div>
</template>

<script>
    export default {
        data(){
            return{
              shop:[
                  {
                      title: "网站首页",
                      icon: "ios-home-outline",
                  },
                  {
                      title:"机构设置",
                      icon:"ios-card-outline"
                  },
                  {
                      title:"分局概况",
                      icon:"md-book"
                  },

                  {
                      title:"分局文件",
                      icon:"md-heart-outline"
                  },
                  {
                      title:"巡视巡察",
                      icon:"ios-list"
                  },
                  {
                      title:"图片视频",
                      icon:"ios-hammer-outline"
                  },
                  {
                      title:"业务之窗",
                      icon:"ios-leaf-outline"
                  },
                  {
                      title:"工作动态",
                      icon:"ios-image-outline"
                  },
                  ],

            }
        }
    }
</script>

<style scoped>
    a{
        color:#333
    }
    ul li{
        list-style: none;
    }
.navigate{

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
        color:#fff;
        font-size: 18px;
        font-weight: 600;

    }
    .navigate .in a span:hover{
        color:#ff0000
    }
    .navigate .in a .ii{
        font-size:30px;
        display: inline-block;
        vertical-align: middle;
        margin-right: 5px;
    }
</style>