<template>
  <div class="box">
    <el-col :span="12">
      <el-menu style="width: 200px"
        default-active="2"
        class="el-menu-vertical-demo"
        @open="handleOpen"
        @close="handleClose">
        <el-menu-item index="1">
            <i class="el-icon-location"></i>
            <span>首页</span>
        </el-menu-item>
        <el-menu-item index="2">
          <i class="el-icon-menu"></i>
          <span slot="title">监测站点</span>
        </el-menu-item>
        <el-menu-item index="3" >
          <i class="el-icon-document"></i>
          <span slot="title">查询</span>
        </el-menu-item>
        <el-menu-item index="4">
          <i class="el-icon-setting"></i>
          <span slot="title">数据服务</span>
        </el-menu-item>
      </el-menu>
    </el-col>
  </div>
</template>

<script type="text/ecmascript-6">
export default {
  methods: {
    handleOpen (key, keyPath) {
    },
    handleClose (key, keyPath) {
    }
  }
};
</script>

<style scoped type="text/css">
</style>
