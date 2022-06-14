<template>
  <div class="header">
    <img width="140px" src="~/assets/logo.svg" />
    <div class="menu">
      <el-menu
        :default-active="activeIndex"
        class="el-menu-demo"
        mode="horizontal"
        @select="handleSelect"
      >
        <el-menu-item index="1">首页</el-menu-item>
        <el-submenu index="2">
          <template slot="title">服务项目</template>
          <el-menu-item index="2-1">选项1</el-menu-item>
          <el-menu-item index="2-2">选项2</el-menu-item>
          <el-menu-item index="2-3">选项3</el-menu-item>
        </el-submenu>
        <el-menu-item index="3">新闻中心</el-menu-item>
        <el-menu-item index="4">关于我们</el-menu-item>
       
        <el-menu-item index="6">联系我们</el-menu-item>
      </el-menu>
    </div>
  </div>
</template>

<script lang='ts'>
export default {};
</script>

<style lang="scss" scoped>
.header {
  height: 90px;
  display: flex;
  align-items: center;
  img {
    object-fit: contain;
    margin: 0 80px;
  }
  .el-menu.el-menu--horizontal {
    border-bottom: none;
  }
  .menu {
    margin-left: auto;
    margin-right: 70px;
  }
}
</style>