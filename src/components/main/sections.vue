<template>
    <div style="height:5000px">
       <div class="banner2" >
           <div >
               <img src="../../assets/images/banner1.jpg" alt="">
           </div>
       </div>
        <div class=" carousel2">
          <div ><img src="../../assets/images/zhuanti.jpg" alt=""></div>
            <div class="list">
              <div style="width:1048px;overflow: hidden">
                 <div>
                     <ul style="display: flex">
                         <li><a href="#"><img src="../../assets/images/z1.jpg" alt=""></a></li>
                         <li><a href="#"><img src="../../assets/images/z2.jpg" alt=""></a></li>
                     </ul>
                 </div>
              </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "section.vue"
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