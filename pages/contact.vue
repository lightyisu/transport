<template>
  <div class="wrapper">
    <div class="banner">
      <div class="text"></div>
    </div>
    <div class="content">
            <el-breadcrumb separator-class="el-icon-arrow-right">
        <el-breadcrumb-item :to="{ path: '/' }">首页</el-breadcrumb-item>
        <el-breadcrumb-item>关于我们</el-breadcrumb-item>
      </el-breadcrumb>
        <div>
            <h3 class="title">联系我们</h3>
            <p>深圳市君悦国际货运代理有限公司</p>
            <p>公司座机：0755-23213032</p>
        </div>
    </div>

  </div>
</template>

<script>
export default {

}
</script>
<style lang="scss" scoped>
.title{
    font-size: 30px;
}
.banner {
  justify-content: center;
  display: flex;
  align-items: center;

  background: url("http://www.szjunyue56.com/upload/img/20190531152317.jpg")
    no-repeat;
  h2 {
    font-size: 45px;
    margin: 0;
    text-align: center;
    color: #fff;
  }
  p {
    color: #fff;
  }
  .text {
    display: inline-block;
  }
  width: 100%;
  background-size: 100% 100%;
  height: 220px;
  border-bottom: 4px solid rgb(243, 203, 175);
}
.content{
    padding: 70px;
}
</style>