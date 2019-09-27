<template>
  <div class="index-warp">
    <div class="index-head w">
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
    </div>
    <div class="index-brnner">
        <el-carousel :interval="5000" arrow="always" height="400px" indicator-position = "none">
          <el-carousel-item>
            <div id="video1"><video ref="video1" src="../assets/MP4/5whhh.mp4"  autoPlay loop style="width= 100%; height=100%; object-fit: fill" width="100%" height="400" @mouseenter="play()" @mouseleave="pause()"> </video></div>
            <div id="video2"><video src="../assets/MP4/5whhh.mp4" controls autoPlay loop style="width= 100%; height=100%; object-fit: fill" height="300" width="100%"> </video></div>
          </el-carousel-item>
          <el-carousel-item>
            <div id="video1"><video src="../assets/MP4/3light.mp4" controls autoPlay loop style="width= 100%; height=100%; object-fit: fill" width="100%" height="400"> </video></div>
            <div id="video2"><video src="../assets/MP4/3light.mp4" controls autoPlay loop style="width= 100%; height=100%; object-fit: fill" height="300" width="100%"> </video></div>
          </el-carousel-item>
          <el-carousel-item>
           <div id="video1"><video src="../assets/MP4/1n.mp4" controls autoPlay loop style="width= 100%; height=100%; object-fit: fill" width="100%" height="400"> </video></div>
            <div id="video2"><video src="../assets/MP4/1n.mp4" controls autoPlay loop style="width= 100%; height=100%; object-fit: fill" height="300" width="100%"> </video></div>
          </el-carousel-item>
        </el-carousel>
    </div>
    <div class="index-content">
      
    </div>
  </div>
</template>

<script>
export default {
 data () {
   return{}
 },
 mounted () {},
 watch: {},
 methods: {
   play () {
    console.log(this.$refs.video1,'111');
    this.$refs.video1.play()
   },
   pause () {
    // this.$refs.video1.pause()
   }
 },
}
</script>

<style lang="scss">
@import '../assets/scss/index.scss';
</style>
