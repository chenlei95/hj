<template>
  <baidu-map class="baidu" :center="center" :zoom="zoom" @ready="handler"></baidu-map>
</template>
<script>
export default {

  data () {
    return {
      center: {lng: 0, lat: 0},
      zoom: 3};
  },
  methods: {
    handler ({BMap, map}) {
      this.center.lng = 120.054548;
      this.center.lat = 30.385546;
      this.zoom = 15;
      map.enableScrollWheelZoom(true);
    }}};
</script>
<style scoped type="text/css">
  .baidu{
    height: 500px;
  }
</style>
