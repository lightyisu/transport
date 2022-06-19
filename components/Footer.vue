<template>
  <div class="footer">
    <div class="links">
      <span class="title">友情链接:</span>
      <span class="small">XX网</span>
      <div class="clear"></div>
      <hr />
    </div>
    <div class="below_content">
      <div class="about">
        <ul>
          <nuxt-link to="/contact">
             <li>关于我们</li>
          </nuxt-link>
         
          <li>公司简介</li>
          <li>公司资质</li>
            <li>联系我们</li>
        </ul>
        <ul>
          <li>国际快递</li>
          <li>DHL国际快递</li>
            <li>UPS国际快递</li>
            <li>FedEx国际快递</li>
          
        </ul>
        <ul>
          <li>国际专线</li>
          <li>中欧铁路</li>
          <li>中东专线</li>
          <li>电池专线</li>
          <li>化工品专线</li>
        </ul>
      
      </div>
      <div class="info">
        <p>电话</p>
        <p class="tel">0755-23213032</p>
        <p>深圳市君悦国际货运代理有限公司</p>
        <p>联系人：刘璞</p>
        <p>手机：18898836256</p>
        <p>邮箱：827615237@qq.com</p>
        <p>地址：广东深圳</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.footer {
  margin-top: 70px;
  height: 500px;
  background: black;
  color: #fff;
  padding: 40px;
  .below_content {
    display: flex;
    .info {
      margin-top: 30px;
      font-size: 17px;
      p {
        margin: 7px 0px;
      }
      margin-left: auto;
      margin-right: 150px;
      .tel {
        color: green;
        font-size: 40px;
      }
    }
  }
  .links {
    .title {
      font-size: 20px;
    }
    .small {
      color: gray;
    }
    .clear {
      height: 50px;
    }
    hr {
      border-color: rgb(109, 107, 107);
    }
  }
  .about {
    ul {
      vertical-align: top;
      display: inline-block;
      list-style: none;
      li:nth-child(1) {
        color: #fff;
        font-size: 20px;
      }
      li {
        margin: 10px 0;
        color: gray;
      }
    }
  }
}
</style>