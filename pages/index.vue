<template>
  <div class="index-warp">
    <Head class="index-head" />
    <Branner class="index-branner" />
    <Nine />
    <Foot />
  </div>
</template>

<script>
import Head from '../components/Head'
import Branner from '../components/Branner'
import Nine from '../components/Nine'
import Foot from '../components/Foot'
export default {
 components: { Head, Branner, Nine, Foot },
  data() {
    return {
     
    }
  }
}
</script>

<style lang='scss' scope>
.index-warp{
  .index-head{
    position: fixed;
    z-index: 9999;
  }
  .index-branner{
    padding-top: 78px;
  }
}
</style>
