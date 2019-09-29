<template>
  <div class="index-warp">
    <!-- <div class="index-head w">
      <ul class="index-head-ul flex-btw">
        <li>
          <a href="javascript:;">
            <img src="../assets/img/logo.jpg" alt="">
          </a>
        </li>
        <li>
          <a href="javascript:;">BLOG</a>
          <a href="javascript:;">GITHUB</a>
          <a href="javascript:;">HELP</a>
        </li>
      </ul>
    </div> -->
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
   return{}
 },
 mounted () {},
 watch: {},
 methods: {},
}
</script>

<style lang="scss">
@import '../assets/scss/index.scss';
</style>
