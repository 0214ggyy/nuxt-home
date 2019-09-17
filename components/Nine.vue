<template>
  <div class="nine-warp">
    <ul class="w">
        <li v-for="item in nineList" :key="item"><a href="javascript:;"><img :src="item" alt=""></a></li>
    </ul>
  </div>
</template>
<script>
import nine1 from '../assets/img/nine/GridImage-1.png'
import nine2 from '../assets/img/nine/GridImage-2.png'
import nine3 from '../assets/img/nine/GridImage-3.png'
import nine4 from '../assets/img/nine/GridImage-4.png'
import nine5 from '../assets/img/nine/GridImage-5.png'
import nine6 from '../assets/img/nine/GridImage-6.png'
import nine7 from '../assets/img/nine/GridImage-7.png'
import nine8 from '../assets/img/nine/GridImage-8.png'
import nine9 from '../assets/img/nine/GridImage-9.png'
export default {
  data () {
    return {
      nineList: [nine1, nine2, nine3, nine4, nine5, nine6, nine7, nine8, nine9]
    }
  },
  methods: {}
}
</script>
<style lang='scss'>
.nine-warp{
  ul{
    width: 1000px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    li{
      width: 30%;
      margin: 10px 0;
      text-align: center;
      overflow: hidden;
      img{
        transform: all 0.3s;
      }
     &:hover img{
       transform: scale(1.1)
     }
    }
  }
}
</style>
