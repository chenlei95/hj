<template>
  <div id="app">
    <Vheader></Vheader>
    <div class="content">
      <div class="left">
        <Left></Left>
      </div>
      <div class="center">
        <BaiduMap></BaiduMap>
      </div>
      <div class="right">
         监测站点数
      </div>
    </div>
    <router-view></router-view>
  </div>

</template>

<script type="text/ecmascript-6">
import Vheader from './components/header/header';
import BaiduMap from './components/right/map.vue';
import Left from './components/left/left';
export default {
  name: 'App',
  components: {
    Vheader,
    BaiduMap,
    Left
  }
};
</script>

<style type="text/css">
#app {
  display: flex;
  width: 100%;
  flex-flow: column;
}
.content{
  display: flex;
  width: 100%;
  height: 500px;
}
.left{
  width: 200px;
}
  .center{
    flex: 3;
    height: 500px;
    padding-left: 10px;
  }
  .right{
    flex: 1;
    text-align: center;
  }
.bm-view {
  flex: 1;
  width: 100%;
  height: 300px;
}
</style>
