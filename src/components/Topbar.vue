<template>
  <div class="topbar">
    <div class="navbar">
      <el-row>
        <el-col :span="20">
          <el-menu
            class="el-menu-demo"
            mode="horizontal"
            background-color="#006699"
            text-color="#61b9e1"
          >
            <el-menu-item>
              <a href="http://www.whpu.edu.cn/jgsz/yxsz.htm">机构设置</a>
            </el-menu-item>
            <el-menu-item>
              <a href="http://www.whpu.edu.cn/zsjy/zsgz.htm">招生就业</a>
            </el-menu-item>
            <el-menu-item>
              <a href="http://rsc.whpu.edu.cn/jszp.htm">人才招聘</a>
            </el-menu-item>
            <el-menu-item>
              <a href="http://xxgkw.whpu.edu.cn/">信息公开</a>
            </el-menu-item>
            <el-menu-item>
              <a href="http://oa.whpu.edu.cn/">办公系统</a>
            </el-menu-item>
            <el-menu-item>
              <a href="http://mail.whpu.edu.cn/">邮件系统</a>
            </el-menu-item>
            <el-menu-item>
              <a href="http://ztb.whpu.edu.cn/">招标信息</a>
            </el-menu-item>
            <el-menu-item>
              <a href="http://www.lib.whpu.edu.cn/">图书馆</a>
            </el-menu-item>
            <el-menu-item>
              <a href="http://www.whpu.edu.cn/en/">English</a>
            </el-menu-item>
          </el-menu>
        </el-col>
        <el-col :span="4">
          <div class="demo-input-suffix">
            <el-input placeholder="检索..." v-model="input" suffix-icon="el-icon-search" size="mini"></el-input>
          </div>
        </el-col>
      </el-row>
    </div>
    <div class="badgeAndMotto">
      <div class="container">
        <div class="badge">
          <a href="#">
            <img src="../assets/homepage/logo.png">
          </a>
        </div>
        <div class="motto">
          <img src="../assets/homepage/text.gif">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "topbar",
  props: {},
  data() {
    return {
      input: ""
    };
  },
  watch: {},
  computed: {},
  methods: {},
  created() {},
  mounted() {}
};
</script>
<style lang="scss" scoped>
.topbar {
  .navbar {
    background-color: #006699;
    height: 40px;

    .el-row {
      max-width: 1170px;
      margin: 0 auto;
      .el-menu--horizontal {
        border-bottom: 0px;
        padding: 0 13px;
        .el-menu-item {
          height: 40px;
          line-height: 40px;
          border-bottom: 0px;
          padding: 0 5px;
          &:hover {
            background-color: #41aadf;
            color: #fff;
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
      }
      .demo-input-suffix {
        height: 40px;
        width: 135px;
        display: flex;
        align-items: center;
        .el-input {
          right: -40px;
        }
        /deep/ .el-input__inner {
          background: #b6d2e1;
          height: 20px;
          border-radius: 10px;
        }
        /deep/ .el-input__inner::-webkit-input-placeholder {
          color: #666666;
        }
        /deep/ .el-input__suffix {
          top: -3px;
        }
        /deep/ .el-input__suffix-inner {
          color: #006699;
        }
      }
    }
  }
  .badgeAndMotto {
    width: 100%;
    height: 142px;
    background: #1295d8 url(../assets/homepage/back2.png) top left repeat;
    text-align: center;
    padding: 15px;
    .container {
      max-width: 1170px;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      .badge {
        margin: 6px 15px;
      }
      .motto {
        margin: 15px 0 15px;
      }
    }
  }

}
</style>


