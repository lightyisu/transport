<template>
  <div>
 

    <section class="wrapper">
      <el-carousel
        data-aos="fade-up"
        data-aos-duration="1000"
        style="width: 1900px; height: 480px"
        height="480px"
      >
        <el-carousel-item v-for="item in carouselImg" :key="item">
          <img class="carousel_img" :src="item" />
        </el-carousel-item>
      </el-carousel>
      <div class="service">
        <h3 class="title" data-aos="fade-up" data-aos-duration="1000">
          我们的服务
        </h3>
        <p data-aos="fade-up" data-aos-duration="1000">
          国际快递 | 国际专线 | 亚马逊FBA | 空运海派
        </p>
        <div data-aos="fade-up" data-aos-duration="1000" class="imgs">
          <div class="block" v-for="fit in 6" :key="fit">
            <p class="desc">3123</p>
            <el-image
              class="flag_imgs"
              style="width: 300px; height: 200px; margin: 30px"
              :src="require('~/assets/img1.jpg')"
              fit="fill"
            >
            </el-image>
          </div>
        </div>
        <div>
          <el-button type="info">查看更多 >></el-button>
        </div>
      </div>
      <div data-aos="fade-up" data-aos-duration="1000" class="info1">
        <h3 class="title" data-aos="fade-up" data-aos-duration="1000">
          渠道优势
        </h3>
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
            <img src="http://www.szjunyue56.com/upload/20190531141759.png" />
          </div>

          <div class="text">
            <h4>安全快捷</h4>
            <p>货物实时跟踪，运输过程全线可查，安全快捷到达FBA仓库</p>
          </div>
        </div>
        <div class="item p3">
          <div class="img-wrapper">
            <img src="http://www.szjunyue56.com/upload/20190531141742.png" />
          </div>

          <div class="text">
            <h4>发货标准化</h4>
            <p>专人管理，流程、交接标准化，货物摆放分配统一化</p>
          </div>
        </div>
        <div class="item p4">
          <div class="img-wrapper">
            <img src="http://www.szjunyue56.com/upload/20190531141724.png" />
          </div>

          <div class="text">
            <h4>运输能力</h4>
            <p>
              公司专业从事FBA跨境电商，国外各地货物运输，有着严谨的运输组织，是一家专业的跨境电商运输公司
            </p>
          </div>
        </div>
        <div class="item p5">
          <div class="img-wrapper">
            <img src="http://www.szjunyue56.com/upload/20190531141706.png" />
          </div>

          <div class="text">
            <h4>服务范围</h4>
            <p>
              君悦国际针对亚马逊FBA专线双清关等业务范围，还针对不同行业，不同目的地，不同业务类别做出具体解决方案
            </p>
          </div>
        </div>
        <div class="item p6">
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
        <h3 class="title" data-aos="fade-up" data-aos-duration="1000">
          服务流程
        </h3>
        <div class="process_card" data-aos="fade-up" data-aos-duration="1000">
          <div class="process_wrapper" v-for="o in 6" :key="o">
            <el-card style="width: 200px" shadow="hover" class="box-card">
              <div class="text item">
                <img
                  src="http://12448.aly17.demo3w.com/upload/20190531142449150.png"
                />
                <p>收货、分拣、包装</p>
              </div>
            </el-card>
            <span v-if="o != 6" class="arrow"></span>
          </div>
        </div>
      </div>
      <div data-aos="fade-up" data-aos-duration="1000" class="info3">
        <div class="text">
          <h2 data-aos="fade-up" data-aos-duration="1000">君悦国际货运代理</h2>
          <p>
            专业从事第三方综合物流服务的运营商，以成为"全球化供应链管理公司"为战略目标
          </p>
        </div>
        <el-button type="success" round>在线咨询</el-button>
      </div>
      <div class="info4">
        <el-card
          data-aos="fade-up"
          data-aos-duration="1000"
          class="box_card"
          v-for="i in 3"
          :key="i"
          :body-style="{ padding: '0px' }"
        >
          <img
            src="http://12448.aly17.demo3w.com/upload/20190611095004.jpg"
            class="image"
          />
          <div style="padding: 14px">
            <h3>墨西哥FBA空运</h3>
            <p>
              意大利FBA空运是君悦国际物流与世界各个优质航空公司合作的一项国际专线服务，该服务结合优质空运公司、清关公司、快递服务商，强强联合，共同打造出时效快、清关强、渠道安全的跨境电商专线服务。
            </p>
            <hr />
            More+
          </div>
        </el-card>

        <div class="more">
          <el-button type="info">查看更多 >></el-button>
        </div>
      </div>
      <div data-aos="fade-up" data-aos-duration="1000" class="info5">
        <h1 data-aos="fade-up" data-aos-duration="1000">其他优势</h1>
        <p>OTHER ADVANTAGES</p>
        <div class="item p1">
          <div class="img-wrapper">
            <img src="http://www.szjunyue56.com/upload/20190531144546.png" />
          </div>

          <div class="text">
            <h4>佳和运通</h4>
            <p>可满足国内直发、FBA或海外仓发货需求</p>
          </div>
        </div>
          <div class="item p2">
          <div class="img-wrapper">
            <img src="http://www.szjunyue56.com/upload/20190531144511.png" />
          </div>

          <div class="text">
               <h4>佳和运通</h4>
            <p>可满足国内直发、FBA或海外仓发货需求</p>
          </div>
        </div>
      </div>
      <div data-aos="fade-up" data-aos-duration="1000" class="info6">
        <h3 class="title">新闻中心</h3>
        <div class="content">
          <el-carousel style="width: 440px" height="400px">
            <el-carousel-item v-for="item in info6.carousel" :key="item">
              <el-card class="play_card" :body-style="{ padding: '0px' }">
                <img
                  :src=item.img
                  class="image"
                />
                <div class="carousel_text" style="padding: 14px">
                  <h4>{{item.title}}</h4>
                  <p>{{item.desc}}</p>

                </div>
              </el-card>
            </el-carousel-item>
          </el-carousel>
          <div class="cards">
            <el-card v-for="item in info6.carousel" :key="item"  class="box-card" shadow="hover"> 
              <h2>{{item.title}}</h2>
              <p>{{item.desc}}</p>
              </el-card>
          
          </div>
        </div>
        <div class="more">
          <el-button type="info">查看更多 >></el-button>
        </div>
      </div>
    </section>
   
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import AOS from "aos";
import "aos/dist/aos.css"; // You can also use <link> for styles
export default Vue.extend({
  name: "IndexPage",
  data() {
    return {
      fits: ["fill", "contain", "cover", "none", "scale-down"],
      url: "../assets/img1.jpg",
      carouselImg: [
        "http://www.szjunyue56.com/upload/img/20190603111643.jpg",
        "http://www.szjunyue56.com/upload/img/20190731115430.jpg",
        "http://www.szjunyue56.com/upload/img/20190603111639.jpg",
      ],
      info6:{
        carousel:[
          {img:'http://www.szjunyue56.com/upload/20190603124450.jpg',title:'发欧洲FBA头程要谨防FBA拒收',desc:'除了清关查验、物流丢包等不可控因素，还要谨防被FBA拒收，发生查验延迟和丢包还可以找货代赔偿，被FBA拒收，基本上就要卖家自己掏腰包了，为此，卖家在打包发货时一定要谨慎。'},
          {
            img:'http://www.szjunyue56.com/upload/20190603124441.jpg',
            title:'亚马逊FBA对这些卖家免收月度仓储费和移除费',
            desc:'亚马逊FBA对这些卖家免收月度仓储费和移除费'
          },
          {
            img:'http://www.szjunyue56.com/upload/20190603124432.jpg',
            title:'中欧班列累计开行超1.4万列',
            desc:'中欧班列累计开行超1.4万列'
          }
        ]
      }
    };
  },
  mounted() {
    AOS.init();
  },
});
</script>
<style lang="scss" scoped>
footer {
  height: 400px;
  width: 1005;
}
.carousel_img {
  width: 100%;
  height: 480px;
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
.info6 {
  text-align: center;
  .image{
    height: 250px;
    width: 100%;
  }

  .content {
    display: flex;
    .play_card {
      height: 100%;
      background: #fff;

    }
    .box-card {
      h2,p{
        margin: 0;
        text-align: left;
      }
      height: 110px;
      margin-bottom: 30px !important;
      width: 800px;
      margin: 0 40px;
    }
  }
  h4{
    margin: 0;
  }
  .carousel_text{
  
    text-align: left;
    height: fit-content;
  }
}
.info5 {
  color: #fff;
  text-align: center;
  position: relative;
  .p2{
    right: 5%;
  }
  .p1 {
    left: 5%;
  }
  .item {
    display: inline-block;
    position: absolute;
    text-align: left;
    .img-wrapper {
      width: 60px;
      height: 60px;
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
      p {
        font-size: 14px;
      }
    }

    background: url("http://12448.aly17.demo3w.com/images/yousitem.png");

    height: 130px;
    background-repeat: no-repeat;
    background-size: 100% 100%;
    width: 400px;
    color: #fff;
  }

  h1 {
    margin: 0;
    margin-top: 40px;
    font-size: 40px;
  }
  p {
    margin: 0;
    font-size: 20px;
    color: gray;
    font-weight: bold;
  }
  height: 400px;
  background-repeat: no-repeat;
  background-size: 100%;
  width: 100%;
  margin: 40px 0;
  background: url("http://12448.aly17.demo3w.com/images/patent.jpg");
}
.info4 {
  display: flex;
  flex-wrap: wrap;
  .more {
    text-align: center;
    width: 100%;
  }
  .box_card {
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
    clear: both;
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
  .process_wrapper {
    display: flex;
  }
  .arrow {
    background: url("http://www.szjunyue56.com/images/jtou.png") no-repeat
      center;

    line-height: 171px;
    width: 36px;
    height: 188px;

    float: left;
    display: block;
  }
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
  .p6 {
    right: 10%;
    top: 70%;
  }
  .p5 {
    left: 10%;
    top: 70%;
  }
  .p4 {
    right: 8%;
    top: 45%;
  }
  .p3 {
    left: 8%;
    top: 45%;
  }
  .p2 {
    right: 10%;
    top: 20%;
  }
  .p1 {
    left: 10%;
    top: 20%;
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
  .block {
    position: relative;
  }
  .desc {
    position: absolute;
    top: 20px;
    color: yellow;
    z-index: 100;
    left: 40px;
  }
  .flag_imgs {
    border: 1px solid black;
    position: relative;
  }

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

