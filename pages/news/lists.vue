<template>
  <div class="wrapper">
    <div class="banner">
      <div class="text"></div>
    </div>
    <div class="content">
      <el-breadcrumb separator-class="el-icon-arrow-right">
        <el-breadcrumb-item :to="{ path: '/' }">首页</el-breadcrumb-item>
        <el-breadcrumb-item>新闻中心</el-breadcrumb-item>
      </el-breadcrumb>
      <div class="lists">
        <Nuxt-link to="/news/detail/2">
                   <el-card shadow="hover" class="box-card">
            <div class="left">

                <img src="http://www.szjunyue56.com/upload/20190603124458.jpg"/>
                <div class="text">
                         <h3>出口“俄罗斯”“英国”“德国”需注意的海关新规</h3>
                         <p>根据俄罗斯海关要求，所有至俄罗斯以及在此中转的货物必须提供6位HS CODE。如果是多种货物混装，涉及到不同的HS CODE，请按照HS CODE分开发送货物信息，避免申报不全，引起海关罚金。</p>
                </div>
           
            </div>
            <div class="right">
                <p>2022</p>
                <p>6-19</p>
            </div>
      </el-card>
        </Nuxt-link>
   
      </div>

    
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.content {
  padding: 70px;
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
.lists{
   ::v-deep .el-card__body{
        display: flex !important;
    }
    margin: 20px 0;
    white-space: pre-line;
    .left{
        width: 70%;
        display: flex;
        img{
            width: 250px;
        }
    }
    .right{
        padding-top: 60px; 
        p{
            margin:0;
            font-size: 30px;
            color: gray;
        }
            width: 300px;
            text-align: center;
            border-left: 1px solid rgb(215, 215, 215);
            display: inline-block;
    }

    .text{
        
        padding: 20px;
        p{
            color: gray;
        }
    }
}
a{
    text-decoration: none;
}
</style>