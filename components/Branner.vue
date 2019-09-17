<template>
    <div class="banner-warp">
        <el-carousel :interval="4000" type="card" height="200">
            <el-carousel-item v-for="item in bannerList" :key="item">
            <img :src="item" alt="">
            </el-carousel-item>
        </el-carousel>
    </div>
</template>
<script>
import banner1 from '../assets/img/branner/banner1.jpg'
import banner2 from '../assets/img/branner/banner2.jpg'
import banner3 from '../assets/img/branner/banner3.jpg'
import banner4 from '../assets/img/branner/banner4.jpg'
import banner5 from '../assets/img/branner/banner5.jpg'
import banner6 from '../assets/img/branner/banner6.jpg'
export default {
  data () {
    return {
      bannerList: [banner1, banner2, banner3, banner4, banner5, banner6]
    }
  }
}
</script>
<style lang='scss'>
.banner-warp{
    background-color: #ffae00;
   .el-carousel__item img {
    width: 100%;
  }
} 
</style>