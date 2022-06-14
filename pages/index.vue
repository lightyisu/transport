<template>
  <div>
    <Header />
    <el-carousel height="500px">
      <el-carousel-item v-for="item in 4" :key="item">
        <h3>{{ item }}</h3>
      </el-carousel-item>
    </el-carousel>
    <section class="wrapper">
      <div class="service">
        <h3 class="title">我们的服务</h3>
        <p>墨西哥空运 | 墨西哥海运 | FBA头程运输 | 海外仓</p>
        <div class="imgs">
          <div class="block" v-for="fit in 6" :key="fit">
            <el-image
              style="width: 300px; height: 200px; margin: 30px"
              :src="require('~/assets/img1.jpg')"
              fit="fill"
            ></el-image>
          </div>
        </div>
        <div>
          <el-button type="info">查看更多 >></el-button>
        </div>
      </div>
      <div class="info1">
        <h3 class="title">渠道优势</h3>
        <div class="item p1">
          <div class="img-wrapper">
            <img
              src="http://12448.aly17.demo3w.com/upload/20190531141817.png"
            />
          </div>

          <div class="text">
            <h4>专线直达</h4>
            <p>君悦国际专注FBA头程，一条龙服务，实行一站式专线运输</p>
          </div>
        </div>
        <div class="item p2">
          <div class="img-wrapper">
            <img
              src="http://12448.aly17.demo3w.com/upload/20190531141817.png"
            />
          </div>

          <div class="text">
            <h4>专线直达</h4>
            <p>君悦国际专注FBA头程，一条龙服务，实行一站式专线运输</p>
          </div>
        </div>
        <div class="center"></div>
      </div>
      <div class="info2">
        <h3 class="title">服务流程</h3>
        <div class="process_card">
          <el-card
            style="width: 200px; margin: 0 20px"
            v-for="o in 6"
            :key="o"
            shadow="hover"
            class="box-card"
          >
            <div class="text item">
              <img
                src="http://12448.aly17.demo3w.com/upload/20190531142449150.png"
              />
              <p>收货、分拣、包装</p>
            </div>
          </el-card>
        </div>
      </div>
      <div class="info3">
        <div class="text">
          <h2>君悦国际货运代理</h2>
          <p>
            专业从事第三方综合物流服务的运营商，以成为"全球化供应链管理公司"为战略目标
          </p>
        </div>
        <el-button type="success" round>在线咨询</el-button>
      </div>
      <div class="info4">
        <el-card class="box_card" v-for="i in 3" :key="i" :body-style="{ padding: '0px' }">
          <img
            src="http://12448.aly17.demo3w.com/upload/20190611095004.jpg"
            class="image"
          />
          <div style="padding: 14px">
            <h3>墨西哥FBA空运</h3>
            <p>意大利FBA空运是君悦国际物流与世界各个优质航空公司合作的一项国际专线服务，该服务结合优质空运公司、清关公司、快递服务商，强强联合，共同打造出时效快、清关强、渠道安全的跨境电商专线服务。</p>
            <hr/>
            More+
          
          </div>
        </el-card>
      
         <div class="more">
          <el-button type="info">查看更多 >></el-button>
        </div>
      </div>
      <div class="info5">
          <h1>其他优势</h1>
          <p>OTHER ADVANTAGES</p>
      </div>
      <div class="info6">
          <h3 class="title">新闻中心</h3>
      </div>
    </section>
    <footer></footer>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "IndexPage",
  data() {
    return {
      fits: ["fill", "contain", "cover", "none", "scale-down"],
      url: "../assets/img1.jpg",
    };
  },
});
</script>
<style lang="scss" scoped>
footer {
  height: 400px;
  width: 1005;
}
.el-carousel__item h3 {
  color: #929598;
  font-size: 18px;
  opacity: 0.75;
  line-height: 300px;
  margin: 0;
}

.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n + 1) {
  background-color: #d3dce6;
}
.info6{
  text-align: center;
}
.info5{
  color: #fff;
  text-align: center;
  
  h1{
    margin: 0;
    margin-top: 40px;
    font-size: 40px;
  }
  p{
    margin: 0;
    font-size: 20px;
    color: gray;
    font-weight: bold;
  }
  height: 400px;
  background-repeat: no-repeat;
  background-size: 100% ;
  width: 100%;
  margin: 40px 0;
  background: url('http://12448.aly17.demo3w.com/images/patent.jpg');
}
.info4{
  display: flex;
  flex-wrap: wrap;
  .more{
    text-align: center;
    width: 100%;
  }
  .box_card{
    width: 400px;
    height: 450px;
    margin: 90px 20px;
  }
    .time {
    font-size: 13px;
    color: #999;
  }
  
  .bottom {
    margin-top: 13px;
    line-height: 12px;
  }

  .button {
    padding: 0;
    float: right;
  }

  .image {
    width: 100%;
    display: block;
  }

  .clearfix:before,
  .clearfix:after {
      display: table;
      content: "";
  }
  
  .clearfix:after {
      clear: both
  }
}
.info3 {
  width: 100%;
  color: #fff;
  height: 220px;
  background: url("http://12448.aly17.demo3w.com/images/xunpan.jpg");
  background-size: 100% 100%;
  background-repeat: no-repeat;
  text-align: center;

  .text {
    text-align: left;
    margin: 80px 0;
    margin-right: 140px;
    display: inline-block;
    h2 {
      font-size: 40px;
      margin: 0;
    }
    p {
      font-size: 20px;
      margin: 0;
    }
  }
}
.info2 {
  width: 100%;
  text-align: center;
  height: 500px;
  .process_card {
    display: flex;
    justify-content: center;
  }
  .box-card {
    background: rgb(223, 223, 223);
  }
}
.info1 {
  background: url("../assets/iyoushi.jpg");
  height: 800px;
  width: 100%;
  margin: 40px 0;
  position: relative;
  text-align: center;

  h3 {
    text-align: center;
    color: #fff;
  }
  .p2 {
    left: 60%;
    top: 30%;
  }
  .p1 {
    left: 12%;
    top: 30%;
  }
  .item {
    display: inline-block;
    position: absolute;
    text-align: left;
    .img-wrapper {
      width: 50px;
      height: 50px;
      position: absolute;
      left: 50px;
      top: 40px;
      overflow: hidden;
    }
    img {
      margin-right: 40px;
    }
    .text {
      width: 240px;
      margin-left: 150px;
    }

    background: url("http://12448.aly17.demo3w.com/images/yousitem.png");

    height: 130px;
    background-repeat: no-repeat;
    background-size: 100% 100%;
    width: 400px;
    color: #fff;
  }
  .center {
    width: 370px;
    position: absolute;
    top: 30%;
    left: 38%;
    background: url("http://12448.aly17.demo3w.com/images/bieshu.png");
    height: 320px;
    background-size: 100% 100%;
  }
}
.wrapper {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  .title {
    width: 1200px;
    display: inline-block;
    margin: 80px 0;
    background: url("~/assets/title.png");
    height: 20px;
    background-repeat: no-repeat;
    font-size: 25px;
    vertical-align: text-top;
    padding-bottom: 20px;
  }
}
.service {
  height: 800px;
  text-align: center;
  width: 1200px;

  .info1 {
    height: 400px;
  }
  .imgs {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
}
</style>

