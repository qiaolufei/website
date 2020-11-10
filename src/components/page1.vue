<template>
  <div class="index__page1">
    <div class="index__page1-head">
      <el-row type="flex" :gutter="20" justify="center">
        <el-col :span="4"
          ><span class="index__page1-head__name">{{name}}</span></el-col
        >
        <el-col :span="9"></el-col>
        <el-col v-for="item in menus" :key="item.name" :span="3"
          ><span @click="goto(item.url)" class="index__page1-head__choose"
            >{{item.name}}</span
          ></el-col>
      </el-row>
    </div>
    <div class="index__page1-main">
      <div class="index__page1-main__name">{{info.name}}</div>
      <div class="index__page1-main__info">{{info.msg1}}</div>
      <div class="index__page1-main__info">{{info.msg2}}</div>
      <div class="index__page1-main__btns">
        <button @click="goto('page5')" class="index__page1-main__btns-left">
          了解我们
        </button>
        <button @click="goto('page6')" class="index__page1-main__btns-right">
          联系我们
        </button>
      </div>
    </div>
    <div class="index__page1-bottom">
      <i
        @click="goto('page2')"
        style="cursor: pointer"
        class="el-icon-arrow-down"
      ></i>
    </div>
  </div>
</template>
<script>
export default {
  data: () => ({
    name: '蜜蜂自习',
    menus: [{name: '蜜蜂自习室', url: 'page2'}, {name: '蜂巢开发小组', url: 'page5'}, {name: '联系我们', url: 'page6'}],
    info: {
      name: '蜜蜂自习',
      msg1: '济南自习室门类销量TOP1',
      msg2: '安静、舒适、饮品免费'
    }
  }),
  methods: {
    goto (id) {
      document.querySelector('#' + id).scrollIntoView(true)
    }
  }
}
</script>
<style lang="less">
.index {
  &__page1 {
    height: 100vh;
    box-sizing: border-box;
    background-position: center;
    background: url(../imgs/page11.jpg) no-repeat;
    background-size: 100% 100%;
    border-radius: 0 0 30% 30%;
    &-head {
      padding-top: 4.4rem;
      &__name,
      &__choose {
        font-size: 3rem;
        line-height: 4rem;
        font-weight: 400;
        color: #000000;
        cursor: pointer;
        white-space: nowrap;
      }
      &__choose {
        font-size: 2.4rem;
      }
    }
    &-main {
      position: absolute;
      left: 50%;
      top: 50%;
      transform: translate(-50%, -50%);
      text-align: center;
      &__name {
        font-size: 7.2rem;
        font-weight: 600;
        line-height: 10rem;
        letter-spacing: 5rem;
        text-indent: 5rem;
        color: #000000;
      }
      &__info {
        font-size: 2.4rem;
        font-weight: 400;
        line-height: 4rem;
        color: #000000;
        letter-spacing: 0.5rem;
        text-indent: 0.5rem;
      }
      &__btns {
        margin-top: 3.7rem;
        &-left,
        &-right {
          width: 20rem;
          height: 6rem;
          border-radius: 1rem;
          font-size: 1.8rem;
          font-weight: 600;
          color: #000000;
          border: none;
        }
        &-left {
          cursor: pointer;
          background: #03004d;
          color: #fff;
        }
        &-right {
          cursor: pointer;
          margin-left: 1.8rem;
          background: #fff;
          color: #03004d;
        }
      }
    }
    &-bottom {
      text-align: center;
      position: absolute;
      bottom: 5rem;
      left: 50%;
      font-size: 2rem;
    }
  }
}
</style>
