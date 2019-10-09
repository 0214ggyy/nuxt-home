<template>
  <div class="index-warp">
    <Head></Head>
    <div class="index-brnner">
        <el-carousel :interval="5000" arrow="never" height="600px" indicator-position = "none">
          <el-carousel-item>
            <video ref="video1" src="../assets/MP4/5whhh.mp4" muted autoPlay loop style="width= 100%; height=100%; object-fit: fill" width="100%" height="600"> </video>
          </el-carousel-item>
          <el-carousel-item>
           <video src="../assets/MP4/3light.mp4" muted  autoPlay loop style="width= 100%; height=100%; object-fit: fill" width="100%" height="600"> </video>
          </el-carousel-item>
          <el-carousel-item>
           <video src="../assets/MP4/1n.mp4" muted  autoPlay loop style="width= 100%; height=100%; object-fit: fill" width="100%" height="600"> </video>
          </el-carousel-item>
          <el-carousel-item>
           <video src="../assets/MP4/6jzz.mp4" muted  autoPlay loop style="width= 100%; height=100%; object-fit: fill" width="100%" height="600"> </video>
          </el-carousel-item>
          <el-carousel-item>
           <video src="../assets/MP4/4beach.mp4" muted  autoPlay loop style="width= 100%; height=100%; object-fit: fill" width="100%" height="600"> </video>
          </el-carousel-item>
        </el-carousel>
    </div>
    <div class="index-content">
      <div class="index-text">
        <ul>
          <li v-for="(item,index) in imgList" :key="index"><img :src="item.urlimg" alt="">
          <span>法师</span>
          </li>
        </ul>
      </div>
      <div class="index-map">
        <Map></Map>
      </div>
    </div>
    <Foot></Foot>
  </div>
</template>

<script>
import Head from '../components/Head'
import Foot from '../components/Foot'
import Map from '../components/Map'
export default {
 components: {Head, Map, Foot},
 data () {
   return{
     imgList:[
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'},
       {urlimg: 'http://game.gtimg.cn/images/yxzj/img201606/heroimg/106/106.jpg'}
     ]
   }
 },
 mounted () {},
 watch: {},
 methods: {},
}
</script>

<style lang="scss">
@import '../assets/scss/index.scss';
</style>
