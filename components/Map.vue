<template>
   <div class="map" id="container">
   </div>
 </template>
<script>
   export default  {
      data() {
      return {}
      },
      mounted(){
      this.loadmap();     //加载地图和相关组件
      },
      methods:{
         loadmap(){
            const map = new window.AMap.Map('container',{
            zoom:20,
            center: [114.421426,30.472087]
         })
         var marker = new AMap.Marker({
            position: [114.421426,30.472087]
         });
         marker.setMap(map);
         var circle = new AMap.Circle({
            center: [114.421426,30.472087],
            radius: 1000,
            fillOpacity:0.2,
            strokeWeight:1
            })
            circle.setMap(map);
            map.setFitView()
                     //设置介绍信息
            var info = new AMap.InfoWindow({
                     content:"我的位置",
                  offset:new AMap.Pixel(0,-28)
         })
         info.open(map,marker.getPosition())
      }
   }	
}		
</script>
<style lang="scss" scoped>
#container{
   width: 100%;
   height: 300px;
   border: 5px dashed #cccccc;
}
</style>