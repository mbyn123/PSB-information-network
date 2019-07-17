<template>
    <div>
       <div class="bgimg">
           <a href="">
           <img src="../../assets/images/banner2.jpg" alt="">
           </a>
       </div>
       <lists/>

    </div>

</template>

<script>
    import lists from "../component/lists"
    export default {
        components:{
            lists
        }
    }
</script>

<style scoped>
.bgimg{
    width:1200px;
    margin: 0 auto;
    border:1px solid #ccc;
    padding: 10px 0 5px 10px;
    margin-top: 10px;
}
</style>