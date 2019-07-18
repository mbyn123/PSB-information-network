<template>
    <div>

        <Row>
            <Col span="16" offset="4">
            <div class="bannerimg" v-for="value in banner" :key="value.id">
             <a href="#">
             <img :src=value.img >
             </a>
            </div>
            </Col>
        </Row>
       <Lists/>

    </div>

</template>

<script>
    import Lists from "../../components/component/lists"
    export default {
        data(){
            return{
                banner:[
                    {
                        img:require("../../assets/images/banner2.jpg")
                    }
                ]
            }
        },
        components:{
            Lists
        }
    }
</script>

<style scoped>
.bannerimg{
    border:1px solid #ccc;
    padding: 10px;
    margin-top: 10px;

}
.bannerimg img{
    width:100%;
}
</style>