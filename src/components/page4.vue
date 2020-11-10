<template>
  <div class="index__page4">
    <div class="index__page4-head">
      <el-row type="flex">
        <el-col :span="24">
          <div class="index__page4-head__name">
            <span>关于蜜蜂自习运营套件</span>
          </div>
          <div style="margin-top: 12px" class="index__page4-head__info">
            由蜂巢开发小组自主开发的TV端/小程序/前后台系统
          </div>
          <div class="index__page4-head__info">
            以互联网推动实体运营效率提升
          </div>
        </el-col>
      </el-row>
    </div>
    <div class="index__page4-main">
      <div v-for="item in list" :key="item.name" class="index__page4-main__box">
        <div class="index__page4-main__box-icon">
          <span :style="{ background: item.color }"></span>
        </div>
        <div class="index__page4-main__box-name">{{ item.name }}</div>
        <div class="index__page4-main__box-info">
          {{ item.info }}
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data: () => ({
    list: [
      {
        name: 'TV端',
        color: '#01C48D',
        info: ' 这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…'
      },
      {
        name: '小程序',
        color: '#5B53FF',
        info: ' 这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…'
      },
      {
        name: '前后台系统',
        color: '#FDBC2A',
        info: ' 这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…'
      }
    ]
  })
}
</script>
<style lang="less">
.index {
  &__page4 {
    height: 100vh;
    &-head {
      text-align: center;
      margin-top: 10vh;
      &__name {
        font-size: 5.2rem;
        line-height: 7.8rem;
        color: #000000;
        span::after {
          content: "";
          position: absolute;
          top: 5.2rem;
          left: 40%;
          height: 1.4rem;
          width: 42rem;
          background: rgba(240, 176, 0, 0.4);
        }
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
      margin-top: 10vh;
      justify-content: center;
      &__box {
        width: 32rem;
        height: 32rem;
        border: 1px solid #999999;
        background: #ffffff;
        box-shadow: 0px 20px 40px rgba(3, 0, 77, 0.04);
        opacity: 1;
        border-radius: 12px;
        text-align: center;
        padding: 2% 2%;
        box-sizing: border-box;
        &-icon {
          span {
            display: inline-block;
            height: 8rem;
            width: 8rem;
            border-radius: 50%;
          }
        }
        &-name {
          margin-top: 3.2rem;
          font-size: 2.4rem;
          line-height: 2.9rem;
          color: #000000;
          opacity: 1;
        }
        &-info {
          margin-top: 1.6rem;
          font-size: 1.8rem;
          line-height: 3.2rem;
          color: #999999;
          opacity: 1;
        }
      }
      &__box:not(:first-child) {
        margin-left: 3rem;
      }
    }
  }
}
</style>
