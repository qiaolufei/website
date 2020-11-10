<template>
  <div class="index__page3">
    <div class="index__page3-main">
      <el-row type="flex" :gutter="20">
        <el-col :span="12">
          <div style="margin-left: 10vw" class="index__page3-main__left">
            <div class="index__page3-main__left-name">
              <span>{{info.name}}</span>
            </div>
            <div class="index__page3-main__left-shop">{{info.title}}</div>
            <div style="margin-top: 40px" class="index__page3-main__left-place">
              详细地址：
            </div>
            <div class="index__page3-main__left-place">
              {{info.place}}
            </div>
            <div class="index__page3-main__left-msg">
              {{info.msg}}
            </div>
            <button class="index__page1-main__btns-left">前往美团</button>
          </div>
        </el-col>
        <el-col :span="12">
          <div class="index__page2-main__right"></div>
        </el-col>
      </el-row>
    </div>
  </div>
</template>
<script>
export default {
  data: () => ({
    info: {
      name: '蜜蜂自习室Max',
      title: '智慧大厦店',
      place: '山东省济南市历城区洪家楼智慧大厦901',
      msg: '这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…'
    }
  })
}
</script>
<style lang="less">
.index {
  &__page3 {
    height: 100vh;
    &-main {
      margin-top: 20vh;
      &__right {
      }
      &__left {
        &-name {
          span::after {
            content: "";
            position: absolute;
            top: 5.2rem;
            left: 10.5vw;
            height: 1.4rem;
            width: 37rem;
            background: rgba(240, 176, 0, 0.4);
          }
        }
        &-name,
        &-shop {
          white-space: nowrap;
          font-size: 5.2rem;
          font-weight: 400;
          line-height: 7.3rem;
          color: #000000;
        }
        &-place {
          white-space: nowrap;
          font-size: 2.4rem;
          font-weight: 500;
          line-height: 4rem;
          color: #000000;
        }
        &-msg {
          width: 70%;
          font-size: 2rem;
          font-weight: 400;
          line-height: 3.4rem;
          color: #999999;
          margin: 2.8rem 0;
        }
      }
    }
  }
}
</style>
