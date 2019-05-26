<template>
  <div class="footerLinks">
    <el-row class="specialTopic">
      <el-col :span="20" class="cards">
        <el-row>
          <el-col :span="6">
            <div class="hot-post">
              <a href="http://wsyx.whpu.edu.cn/default.html">
                <img src="../assets/homepage/11111.jpg">
                <h3>网上迎新系统</h3>
              </a>
            </div>
          </el-col>
          <el-col :span="6">
            <div class="hot-post">
              <a href="http://sjdztw.whpu.edu.cn/">
                <img src="../assets/homepage/19dazhuanti.jpg">
                <h3>“十九大”专题</h3>
              </a>
            </div>
          </el-col>
          <el-col :span="6">
            <div class="hot-post">
              <a href="http://lxyz.whpu.edu.cn/">
                <img src="../assets/homepage/lxyz.jpg">
                <h3>“两学一做”专题</h3>
              </a>
            </div>
          </el-col>
          <el-col :span="6">
            <div class="hot-post">
              <a href="http://xxgkw.whpu.edu.cn/">
                <img src="../assets/homepage/xxgk.jpg">
                <h3>信息公开网</h3>
              </a>
            </div>
          </el-col>
        </el-row>
      </el-col>
      <el-col :span="4" class="qrcode">
        <el-popover placement="top-start" title="官方微信" width="130" trigger="hover">
          <img
            src="../assets/homepage/qrcode_gh_5d94bd2ccc5f_1.jpg"
            style="width: 130px;height: 130px;"
          >
          <a id="popover-wx" href="#" target="_blank" slot="reference">官方微信</a>
        </el-popover>
        <el-popover placement="top-start" title="官方微博" width="130" trigger="hover">
          <img src="../assets/homepage/weiboerweima_12.png" style="width: 130px;height: 130px;">
          <a id="popover-wb" href="#" target="_blank" slot="reference">官方微博</a>
        </el-popover>
      </el-col>
    </el-row>
    <div class="footer">
      <div class="footerL fl">
        <ul>
          <li>
            <a href="Mailto:secretary@whpu.edu.cn">书记信箱</a>
            <a href="mailto:president@whpu.edu.cn">校长信箱</a>
            <a href="http://xyh.whpu.edu.cn/">校友</a>
            <a href="http://wsb.whpu.edu.cn/">国际学生</a>
            <a href="http://www.whpu.edu.cn/sftd/ksjfk.htm">考生及访客</a>
          </li>
          <li>
            <a href="http://www.whpu.edu.cn/xxgk1/xxjj.htm">学校概况</a>
            <a href="http://www.whpu.edu.cn/rcpy/bksjy.htm">人才培养</a>
            <a href="http://kyc.whpu.edu.cn/">科学研究</a>
            <a href="http://cxyc.whpu.edu.cn/">社会服务</a>
            <a href="http://www.whpu.edu.cn/xywh/sjxxsbxt.htm">校园文化</a>
          </li>
        </ul>
      </div>
      <div class="footerM fl">
        <div class="footerMT hidden-xs hidden-sm">
          <img alt="武汉轻工大学" src="../assets/homepage/footer_logo.png">
        </div>
        <div class="footerMB">
          <p class="name"></p>
          <p class="copright"></p>
          <p>
            版权所有 2016&nbsp;武汉轻工大学&nbsp;鄂ICP备15021561号-1
            <br>
            <a
              target="_blank"
              href="http://www.beian.gov.cn/portal/registerSystemInfo?recordcode=42011202000327"
              style="color:white;"
            >
              <img src="../assets/homepage/beian.png">鄂公网安备42011202000327号
            </a>
          </p>
          <p></p>
          <p class="daohang">
            <a href="http://www.whpu.edu.cn/xxgk1/lxwm.htm">联系我们</a>
            <a
              href="http://news.whpu.edu.cn/tougao.jsp?urltype=tree.TreeTempUrl&amp;wbtreeid=1019"
            >新闻投稿</a>
          </p>
          <p class="daohang">
            <a
              href="http://bszs.conac.cn/sitename?method=show&amp;id=54415C18FF0360F9E053022819AC6AF3"
            >
              <img src="../assets/homepage/bszs.png">
            </a>
          </p>
        </div>
      </div>
      <div class="footerR fr">
        <ul>
          <li>
            <a href="http://zsb.whpu.edu.cn/" target="_blank">招生</a>
            <a href="http://whpu.91wllm.com/" target="_blank">就业</a>
            <a href="http://rsc.whpu.edu.cn/jszp.htm" target="_blank">招聘</a>
            <a href="http://jjh.whpu.edu.cn/" target="_blank">捐赠</a>
          </li>
          <li>
            <a href="http://www.whpu.edu.cn/xxgk1/xxxl.htm" target="_blank">校历</a>
            <a href="#" target="_blank">黄页</a>
            <a href="http://www.lib.whpu.edu.cn/" target="_blank">图书馆</a>
            <a href="#" target="_blank">校园地图</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "footerLinks",
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
.footerLinks {
  .specialTopic {
    max-width: 1170px;
    margin: 0 auto;
    background: #fff;
    margin-top: 15px;
    padding: 0 15px;
    .cards {
      .el-col {
        padding: 0 15px;
        .hot-post {
          overflow: hidden;
          position: relative;
          border-bottom: 1px solid #ededed;
          background: #ededed;
          a {
            text-decoration: none;
            &:hover {
              text-decoration: underline;
            }
            img {
              width: 100%;
              transition: all 0.5s;
              &:hover {
                transform: scale(1.2);
              }
            }
            h3 {
              color: #1295d8;
              font-size: 14px;
              text-transform: uppercase;
              margin: 5px 0 10px;
              text-align: center;
            }
          }
        }
      }
    }
    .qrcode {
      padding: 15px;
      padding-left: 25px;
      a {
        display: block;
        height: 50px;
        line-height: 50px;
        color: #1295d8;
        padding-left: 36px;
        text-decoration: none;
        &:hover {
          text-decoration: underline;
        }
      }
      #popover-wx {
        background: url(../assets/homepage/weixin.png) no-repeat left center;
      }
      #popover-wb {
        background: url(../assets/homepage/weibo.png) no-repeat left center;
      }
    }
  }
  .footer {
    width: 100%;
    height: 240px;
    overflow: hidden;
    background: #2196d5 url(../assets/homepage/back2.png);
    margin-top: 45px;
    padding-bottom: 30px;
    font-size: 12px;
    a {
      text-decoration: none;
      &:hover {
        text-decoration: underline;
      }
    }
    .footerL,
    .footerR {
      padding: 27px 0;
      width: 32%;
    }
    .footerL ul li {
      width: 44%;
      height: 131px;
      border-right: 1px solid #f1f1f1;
      float: left;
      padding: 10px 0;
      list-style: none;
      a {
        display: block;
        text-align: right;
        color: #f1f1f1;
        padding-right: 5px;
        line-height: 22px;
        text-decoration: none;
      }
    }
    .footerR ul li {
      width: 44%;
      height: 131px;
      border-left: 1px solid #f1f1f1;
      float: right;
      padding: 12px 0;
      list-style: none;
      a {
        display: block;
        text-align: left;
        color: #f1f1f1;
        padding-left: 5px;
        line-height: 22px;
        text-decoration: none;
      }
    }
    .fl {
      float: left;
    }
    .fr {
      float: right;
    }
    .footerM {
      width: 36%;
      margin: 18px auto;
      .footerMT {
        img {
          max-width: 321px;
          height: auto;
          display: block;
          margin: 0 auto;
        }
      }
      .footerMB {
        color: #f1f1f1;
        width: 100%;
        p {
          text-align: center;
          padding: 3px 0;
        }
        p.name {
          font-size: 18px;
          line-height: 22px;
          margin-top: 3px;
        }
        p.daohang {
          line-height: 15px;
          a {
            color: #f1f1f1;
            padding-right: 10px;
          }
        }
      }
    }
  }
}
</style>