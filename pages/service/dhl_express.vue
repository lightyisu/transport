<template>
  <div class="wrapper">
    <div class="banner">
      <div class="text">
        <h2>DHL国际专线</h2>
        <p>
          香港直飞航班，货物清关后交当地DHL国际快递派送投递，资费低,
          旺季不排仓，跟踪详细
        </p>
      </div>
    </div>
    <div class="content">
      <el-breadcrumb separator-class="el-icon-arrow-right">
        <el-breadcrumb-item :to="{ path: '/' }">首页</el-breadcrumb-item>
        <el-breadcrumb-item>DHL国际专线，DHL专线 ，DHL快递</el-breadcrumb-item>
      </el-breadcrumb>
      <el-card shadow="never" class="wrapper-card box-card">
        <div class="title">
          <h4>服务概况 Service Overview</h4>
          <hr />
        </div>
        <div class="intro-img">
          <img src="../../assets/dhl_exp.jpg" />
          <p>
          DHL国际专线是忠迅国际物流跟DHL国际快递公司合作，而整合出来的一个超高性价比的空加派服务运输渠道，将货物在国内集中分拣，配载香港直飞航班，货物清关后交当地DHL国际快递派送投递到欧美，东南亚，澳纽，日本，中东，新加波等国家。


主要服务跨境电商群体，ebay，速卖通，Lazada，Wish，Newegg，敦煌，阿里国际，亚马逊，Konga，Jumia，Kilimail，Linio等平台卖家


服务简称

DHL国际专线，DHL专线

DHL国际快递专线，DHL国际快递
          </p>
        </div>
        <div class="title">
          <h4>服务详情 Service Details</h4>
          <hr />
          <p>
          DHL国际专线递送时效

参考时间：2—7工作日

特殊情况除外！派送时效跟目的地各个海关清关时间及航班安排有关。


操作灵活，时效快

全程跟踪，时效快

旺季不排仓，跟踪详细


关税相关

1.以目的国产生的关税为准 (一般是申报价值高的产生的关税比较高，如果申报的价值比实际价值过于低，也会产生比较高的惩罚性关税）。


理赔相关

1.对于少件、缺货、破损的包裹如收件人收到的包裹重量、数量、件数不符、破损的邮包，请收件人收到包裹24小时内向目的地快递的反馈丢失或破损情况。


附加费：偏远费和燃油附加费

关税相关：目的地国家进口可能产生关税

退件相关：提供退件服务


全球化

可接内电、配套、纯电和移动电源


包装要求

请注意包装要完好，不要易破损，在包装袋外侧除地址标签外，尽量不要带其他无关标识，对于易碎品最好外包装上有易碎品的标志，请妥善包装您的包裹以免在运输中损坏。


服务常见问题

1、DHL国际专线禁寄物品有哪些？

可能危害航空安全的物品。

国家法律、邮政法规和海关条例禁止的物品。


2、DHL国际专线几个注意事项

乌克兰、巴西、捷克、波兰、白俄罗斯无弃件服务。俄罗斯能否弃件，需要询当地海关。


3、DHL国际专线运输偏远地方说明？

到巴西一些偏远区或一些没有列明的地区，税款必须由寄件人付。（偏远地区可在DHL官网查询）
          </p>
       
       
        </div>
      </el-card>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.clearfix{
    font-weight: bold;
}
.wrapper {
  word-break: break-all;
  white-space: pre-line;
  word-wrap: break-word;
}
.intro-img {
  display: flex;
  align-items: center;
  img {
    width: 600px;
    float: left;
  }
  p {
    width: 500px;
    margin: 0px 20px;
  }
}
.title {
  h4 {
    margin: 10px 0;

    display: inline-block;
  }
  hr {
    background: rgb(232, 43, 43);
    height: 2px;
  }
}
.banner {
  justify-content: center;
  display: flex;
  align-items: center;

  background: url("https://www.zxgj56.com/Upload/201903/281851595356.jpg")
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
  height: 200px;
  border-bottom: 4px solid rgb(232, 43, 43);
}
.content {
  padding: 70px;
  .wrapper-card {
    margin: 40px 0;
    min-height: 1200px;
  }
  background: rgb(235, 235, 235);
}
.problem .box-card {
  margin: 40px 0;
}
</style>