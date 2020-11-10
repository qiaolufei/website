<template>
  <div class="index__page2" id="page2">
    <div class="index__page2-main">
      <el-row type="flex" :gutter="20">
        <el-col :span="12">
          <div class="index__page2-main__left"></div>
        </el-col>
        <el-col :span="12">
          <div class="index__page2-main__right">
            <div class="index__page2-main__right-name">
              <span>{{info.name}}</span>
            </div>
            <div class="index__page2-main__right-shop">{{info.title}}</div>
            <div
              style="margin-top: 40px"
              class="index__page2-main__right-place"
            >
              详细地址：
            </div>
            <div class="index__page2-main__right-place">
              {{info.place}}
            </div>
            <div class="index__page2-main__right-msg">
              {{info.msg}}
            </div>
            <button class="index__page1-main__btns-left">前往美团</button>
          </div>
        </el-col>
      </el-row>
    </div>
  </div>
</template>
<script>
export default {
  data: () => ({
    info: {
      name: '蜜蜂自习室',
      title: '印象城店',
      place: '山东省济南市历城区隆悦花园4号楼2单元1201',
      msg: '这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…'
    }
  })
}
</script>
<style lang="less">
.index {
  &__page2 {
    height: 100vh;
    padding-top: 20vh;
    &-main {
      &__left {
      }
      &__right {
        &-name {
          span::after {
            content: "";
            position: absolute;
            top: 5.2rem;
            left: 50.6%;
            height: 1.4rem;
            width: 26.2rem;
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
