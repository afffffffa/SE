<template>

  <div class="header">
    <div class="breadcrumb-container">
      <el-breadcrumb separator="/" class="breadcrumb">
        <el-breadcrumb-item :to="{ path: '/index' }"><span class="el-icon-arrow-left iconback"></span> 首页 </el-breadcrumb-item>
        <el-breadcrumb-item>
          <slot name="hname">
            <!-- <span>活动管理</span> -->
          </slot>
        </el-breadcrumb-item>
      </el-breadcrumb>
    </div>
  </div>
</template>
<script>

export default {
  name: 'Header',
  components: {

  }
}
</script>
<style scoped>
.header {
  width: 100%;
}
.breadcrumb-container {
  width: 90%;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  margin-top: 20px;
  margin-right: 5%;
}
.breadcrumb {
  width: 80%;
  font-size: 18px;
}
.iconback {
  margin-right: 10px;
  font-size: 20px;
}
</style>
