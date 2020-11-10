<template>
  <div class="index__page5" id="page5">
    <el-row type="flex">
      <el-col :span="24">
        <div class="index__page5-head">
          <div class="index__page5-head__name">
            蜂巢开发小组<span style="font-size: 40px">
              Hive Developer Team
            </span>
          </div>
          <div class="index__page5-head__name">
            <span>来自北京的一线金融&互联网研发团队</span>
          </div>
          <div class="index__page5-head__info">
            承接各种企业及业务场景的系统开发需求，从源头提升您的效率
          </div>
          <div class="index__page5-head__info">
            小程序、Web、APP开发我们都可以
          </div>
        </div>
        <div class="index__page5-main">
          <div class="index__page5-main__box"></div>
          <div class="index__page5-main__box"></div>
          <div class="index__page5-main__box"></div>
        </div>
      </el-col>
    </el-row>
  </div>
</template>
<script>
export default {
  data: () => ({})
}
</script>
<style lang="less">
.index {
  &__page5 {
    height: 100vh;
    padding: 4% 4%;
    &-head {
      &__name {
        font-size: 5.2rem;
        font-weight: 600;
        line-height: 7.8rem;
        color: #000000;
        opacity: 1;
      }
      &__info {
        font-size: 3rem;
        line-height: 4rem;
        color: #999999;
        opacity: 1;
      }
    }
    &-main {
      display: flex;
      flex-direction: row;
      margin-top: 5vh;
      justify-content: center;
      &__box {
        width: 32rem;
        height: 36rem;
        border: 1px solid #999999;
        background: #ffffff;
        box-shadow: 0px 20px 40px rgba(3, 0, 77, 0.04);
        opacity: 1;
        border-radius: 12px;
        text-align: center;
        padding: 2% 2%;
        box-sizing: border-box;
      }
      &__box:not(:first-child) {
        margin-left: 5rem;
      }
    }
  }
}
</style>
