<template>
  <div class="index__page6" id="page6">
    <div class="index__page6-main">
      <el-row type="flex" :gutter="20">
        <el-col :span="5">
          <div class="index__page6-main__left">
            <div class="index__page6-main__left-name">联系我们</div>
            <div style="margin-top: 37px" class="index__page6-main__left-info">
              {{phone}}
            </div>
            <div style="margin-top: 22px" class="index__page6-main__left-info">
              自习室相关合作&开发合作
            </div>
          </div>
        </el-col>
        <el-col :span="11"></el-col>
        <el-col :span="4">
          <div class="index__page6-main__right">
            <img src="../imgs/wechat.jpg" alt="" />
            <div class="index__page6-main__right-name">个人微信</div>
          </div>
        </el-col>
        <el-col :span="4">
          <div class="index__page6-main__right">
            <img src="../imgs/wechat.jpg" alt="" />
            <div class="index__page6-main__right-name">小程序</div>
          </div>
        </el-col>
      </el-row>
    </div>
    <el-divider></el-divider>
    <div class="index__page6-foot">© 2020 Easy. All right reserved.</div>
  </div>
</template>
<script>
export default {
  data: () => ({
    phone: '(+86) 133 222 53105'
  })
}
</script>
<style lang="less">
.index {
  &__page6 {
    /deep/ .el-divider--horizontal {
      margin: 3rem 0;
    }
    height: 40vh;
    background: #03004d;
    padding: 4% 6%;
    color: #fff;
    &-main {
      &__left {
        &-name {
          font-size: 3rem;
          line-height: 4.8rem;
        }
        &-info {
          font-size: 2rem;
          line-height: 3.2rem;
        }
      }
      &__right {
        text-align: center;
        img {
          width: 13rem;
          height: 13rem;
        }
        &-name {
          margin-top: 2rem;
          font-size: 2rem;
          color: #ffffff;
          opacity: 1;
        }
      }
    }
    &-foot {
      text-align: center;
      font-size: 1.6rem;
      line-height: 10rem;
    }
  }
}
</style>
