<template>
  <div class="container">
    <div class="navMenu">
      <el-row>
        <el-col :span="12">
          <el-menu class="el-menu-demo" mode="horizontal" text-color="#006699">
            <el-submenu index="1">
              <template slot="title">学校概况</template>
              <div class="submenuItem">
                <el-menu-item index="1-1">
                  <a href="http://www.whpu.edu.cn/xxgk1/xxjj.htm">学校简介</a>
                </el-menu-item>
                <el-menu-item index="1-2">
                  <a href="http://www.whpu.edu.cn/xxgk1/xxld.htm">学校领导</a>
                </el-menu-item>
                <el-menu-item index="1-3">
                  <a href="http://www.whpu.edu.cn/xxgk1/xxzc.htm">学校章程</a>
                </el-menu-item>
                <el-menu-item index="1-4">
                  <a href="http://www.whpu.edu.cn/xxgk1/xxxl.htm">学校校历</a>
                </el-menu-item>
                <el-menu-item index="1-5">
                  <a href="http://www.whpu.edu.cn/xxgk1/lxwm.htm">联系我们</a>
                </el-menu-item>
              </div>
            </el-submenu>
            <el-menu-item>
              <a href="http://www.whpu.edu.cn/rcpy/bksjy.htm">人才培养</a>
            </el-menu-item>
            <el-menu-item>
              <a href="http://kyc.whpu.edu.cn/">科学研究</a>
            </el-menu-item>
            <el-menu-item>
              <a href="http://cxyc.whpu.edu.cn/">社会服务</a>
            </el-menu-item>
            <el-menu-item>
              <a href="http://www.whpu.edu.cn/xywh/sjxxsbxt.htm">校园文化</a>
            </el-menu-item>
          </el-menu>
        </el-col>
        <el-col :span="12">
          <el-menu class="el-menu-demo fr" mode="horizontal" text-color="#006699">
            <el-menu-item>
              <a href="mailto:secretary@whpu.edu.cn">书记信箱</a>
            </el-menu-item>
            <el-menu-item>
              <a href="mailto:president@whpu.edu.cn">校长信箱</a>
            </el-menu-item>
            <el-menu-item>
              <a href="http://xyh.whpu.edu.cn/">校友</a>
            </el-menu-item>
            <el-menu-item>
              <a href="http://wsb.whpu.edu.cn/">国际学生</a>
            </el-menu-item>
            <el-menu-item>
              <a href="http://www.whpu.edu.cn/sftd/ksjfk.htm">考生及访客</a>
            </el-menu-item>
            <el-menu-item>
              <a href="http://news.whpu.edu.cn/">学校新闻网</a>
            </el-menu-item>
            <el-menu-item>
              <a href="http://xxbgs.whpu.edu.cn/fwzn/xxbgdh.htm">办公电话</a>
            </el-menu-item>
          </el-menu>
        </el-col>
      </el-row>
    </div>
    <div class="banner">
      <el-carousel height="360px">
        <el-carousel-item>
          <a href="http://www.whpu.edu.cn/">
            <img src="../assets/newsImg/tiaozhanbei.jpg">
          </a>
        </el-carousel-item>
        <el-carousel-item>
          <a href="http://www.whpu.edu.cn/info/1003/11301.htm">
            <img src="../assets/newsImg/taohongdiaoyan.jpg">
          </a>
        </el-carousel-item>
        <el-carousel-item>
          <a href="http://www.whpu.edu.cn/info/1003/11346.htm">
            <img src="../assets/newsImg/liangdaihui.jpg">
          </a>
        </el-carousel-item>
        <el-carousel-item>
          <a href="http://www.whpu.edu.cn/info/1003/11228.htm">
            <img src="../assets/newsImg/guojiajipingtai.jpg">
          </a>
        </el-carousel-item>
        <el-carousel-item>
          <a href="http://www.whpu.edu.cn/">
            <img src="../assets/newsImg/zhuanjiazhuanjia2018.6.23.jpg">
          </a>
        </el-carousel-item>
        <el-carousel-item>
          <a href="https://www.gfbzb.gov.cn/">
            <img src="../assets/newsImg/guofang.jpg">
          </a>
        </el-carousel-item>
      </el-carousel>
    </div>
    <News/>
    <Footer/>
  </div>
</template>

<script>
import News from "./News.vue";
import Footer from "./Footer.vue";
export default {
  name: "container",
  components: {
    News,
    Footer
  },
  props: {},
  data() {
    return {};
  },
  watch: {},
  computed: {},
  methods: {},
  created() {},
  mounted() {}
};
</script>
<style lang="scss" scoped>
.container {
  .navMenu {
    height: 40px;
    background-color: #fff;
    .el-row {
      max-width: 1170px;
      margin: 0 auto;
      .el-menu--horizontal {
        border-bottom: 0px;
        padding: 0 15px;
        /deep/ .el-menu-item,
        /deep/ .el-submenu__title {
          height: 40px;
          line-height: 40px;
          border-bottom: 0px;
          padding: 0 8px;
          &:hover {
            background-color: #006699;
            a {
              color: #fff;
            }
          }
          &.is-active {
            color: #fff;
          }
          a {
            font-size: 13px;
            text-decoration: none;
            text-align: center;
          }
        }
        /deep/ .el-submenu__title:hover {
          background: #fff;
        }
      }
    }
  }
  .banner {
    max-width: 1170px;
    margin: 0 auto;
    img {
      width: 100%;
      height: 360px;
    }
  }
}

</style>

<style lang="scss">
.el-menu--horizontal .el-menu .el-menu-item,
.el-menu--horizontal .el-menu .el-submenu__title {
  height: 40px;
  line-height: 40px;
  border-bottom: 0px;
  padding: 0 5px;
  &:hover {
    background-color: #006699;
    color: #fff;
    a {
      color: #fff;
    }
  }
  &.is-active {
    color: #fff;
  }
  a {
    color: #006699;
    font-size: 13px;
    text-decoration: none;
    text-align: center;
  }
}
.el-menu--popup {
  min-width: 70px;
}
.el-menu-demo.fr {
  float: right;
}
</style>