<template>
  <div class="header">
    <img width="100px" src="~/assets/logo.png" class="logo"/>
    <span class="text">运通佳和</span>
    <div class="menu">
      <el-menu
        :default-active="activeIndex"
        class="el-menu-demo"
        mode="horizontal"
        data-aos="fade-left"
          data-aos-duration="1000"
        @select="handleSelect"
        
      >
        <el-menu-item index="1">
          <Nuxt-link to="/">
            首页
          </Nuxt-link>
          </el-menu-item>
        <el-submenu index="2">
          <template slot="title">国际快递</template>
          <el-menu-item index="2-1">
             <Nuxt-link to="/service/dwadwa">
             DHL快递
          </Nuxt-link>
           </el-menu-item>
          <el-menu-item index="2-2">UPS国际快递</el-menu-item>
          <el-menu-item index="2-3">FedEX国际快递</el-menu-item>
        </el-submenu>
          <el-submenu index="3">
          <template slot="title">国际专线</template>
          <el-menu-item index="2-1">中欧铁路</el-menu-item>
          <el-menu-item index="2-2">澳洲专线</el-menu-item>
          <el-menu-item index="2-3">中东专线</el-menu-item>
            <el-menu-item index="2-4">电池专线</el-menu-item>
          <el-menu-item index="2-5">化工品专线</el-menu-item>
        </el-submenu>
            <el-submenu index="4">
          <template slot="title">亚马逊FBA</template>
          <el-menu-item index="2-1">欧洲FBA</el-menu-item>
          <el-menu-item index="2-2">美国FBA</el-menu-item>
          <el-menu-item index="2-3">澳洲FBA</el-menu-item>
            <el-menu-item index="2-4">亚马逊FBA</el-menu-item>
     
        </el-submenu>
           <el-submenu index="5">
          <template slot="title">空运海派</template>
          <el-menu-item index="2-1">加拿大海运</el-menu-item>
          <el-menu-item index="2-2">美国海运</el-menu-item>
          <el-menu-item index="2-3">欧洲海运</el-menu-item>
            <el-menu-item index="2-4">欧洲空运</el-menu-item>
     
        </el-submenu>
        
        <el-menu-item index="5"><Nuxt-link to="/news/lists">
            新闻中心
          </Nuxt-link></el-menu-item>
        <el-menu-item index="6">关于我们</el-menu-item>
       
      
      </el-menu>
    </div>
  </div>
</template>

<script lang='ts'>
import AOS from 'aos';
import 'aos/dist/aos.css'; // You can also use <link> for styles
export default {
  mounted(){
      AOS.init();
  }
};
</script>

<style lang="scss" scoped>
.text{
  font-size: 23px;
  font-weight: bold;
}
.logo{
  object-fit: contain;
  position: relative;
  top:16px;

}
.header {
  height: 90px;
  display: flex;
  align-items: center;
  img {
    object-fit: contain;
    margin: 0;
    margin-left: 80px;
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