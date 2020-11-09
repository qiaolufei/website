<template>
  <div class="index">
    <div class="index__page1">
      <div class="index__page1-head">
        <el-row type="flex" :gutter="20" justify="center">
          <el-col :span="4"
            ><span class="index__page1-head__name">蜜蜂自习</span></el-col
          >
          <el-col :span="9"></el-col>
          <el-col :span="3"
            ><span class="index__page1-head__choose">蜜蜂自习室</span></el-col
          >
          <el-col :span="3"
            ><span class="index__page1-head__choose">蜂巢开发小组</span></el-col
          >
          <el-col :span="3"
            ><span class="index__page1-head__choose">联系我们</span></el-col
          >
        </el-row>
      </div>
      <div class="index__page1-main">
        <div class="index__page1-main__name">蜜蜂自习</div>
        <div class="index__page1-main__info">济南自习室门类销量TOP1</div>
        <div class="index__page1-main__info">安静、舒适、饮品免费</div>
        <div class="index__page1-main__btns">
          <button class="index__page1-main__btns-left">了解我们</button>
          <button class="index__page1-main__btns-right">联系我们</button>
        </div>
      </div>
      <div class="index__page1-bottom">
        <i class="el-icon-arrow-down"></i>
      </div>
    </div>
    <div class="index__page2">
      <div class="index__page2-main">
        <el-row type="flex" :gutter="20">
          <el-col :span="12">
            <div class="index__page2-main__left"></div>
          </el-col>
          <el-col :span="12">
            <div class="index__page2-main__right">
              <div class="index__page2-main__right-name">
                <span>蜜蜂自习室</span>
              </div>
              <div class="index__page2-main__right-shop">印象城店</div>
              <div
                style="margin-top: 40px"
                class="index__page2-main__right-place"
              >
                详细地址：
              </div>
              <div class="index__page2-main__right-place">
                山东省济南市历城区隆悦花园4号楼2单元1201
              </div>
              <div class="index__page2-main__right-msg">
                这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…
              </div>
              <button class="index__page1-main__btns-left">前往美团</button>
            </div>
          </el-col>
        </el-row>
      </div>
    </div>
    <div class="index__page3">
      <div class="index__page3-main">
        <el-row type="flex" :gutter="20">
          <el-col :span="12">
            <div style="margin-left: 10vw" class="index__page3-main__left">
              <div class="index__page3-main__left-name">
                <span>蜜蜂自习室Max</span>
              </div>
              <div class="index__page3-main__left-shop">智慧大厦店</div>
              <div
                style="margin-top: 40px"
                class="index__page3-main__left-place"
              >
                详细地址：
              </div>
              <div class="index__page3-main__left-place">
                山东省济南市历城区洪家楼智慧大厦901
              </div>
              <div class="index__page3-main__left-msg">
                这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…这里放一篇小作文…
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
        <div
          v-for="item in list"
          :key="item.name"
          class="index__page4-main__box"
        >
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
    <div class="index__page5">
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
    <div class="index__page6"></div>
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
<style lang="less" scoped>
button:focus,
button:active:focus,
button.active:focus,
button.focus,
button:active.focus,
button.active.focus {
  outline: none;
  border-color: transparent; // 若是本身具有 border 请删除此属性
  box-shadow: none;
}
.index {
  box-sizing: border-box;
  &__page1 {
    height: 100vh;
    box-sizing: border-box;
    margin: 0px;
    background-position: center;
    background: url(../imgs/page11.jpg) no-repeat;
    background-size: 100% 100%;
    border-radius: 0 0 30% 30%;
    &-head {
      padding-top: 44px;
      &__name,
      &__choose {
        font-size: 30px;
        line-height: 40px;
        font-weight: 400;
        color: #000000;
        cursor: pointer;
      }
      &__choose {
        font-size: 24px;
      }
    }
    &-main {
      position: absolute;
      left: 50%;
      top: 50%;
      transform: translate(-50%, -50%);
      text-align: center;
      &__name {
        font-size: 72px;
        font-weight: 600;
        line-height: 100px;
        letter-spacing: 50px;
        text-indent: 50px;
        color: #000000;
      }
      &__info {
        font-size: 24px;
        font-weight: 400;
        line-height: 40px;
        color: #000000;
        letter-spacing: 5px;
        text-indent: 5px;
      }
      &__btns {
        margin-top: 37px;
        &-left,
        &-right {
          width: 200px;
          height: 60px;
          border-radius: 10px;
          font-size: 18px;
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
          margin-left: 18px;
          background: #fff;
          color: #03004d;
        }
      }
    }
    &-bottom {
      text-align: center;
      position: absolute;
      bottom: 50px;
      left: 50%;
      font-size: 20px;
    }
  }
  &__page2 {
    border: 1px solid red;
    height: 100vh;
    &-main {
      margin-top: 20vh;
      &__left {
      }
      &__right {
        &-name {
          span::after {
            content: "";
            position: absolute;
            top: 52px;
            left: 50.6%;
            height: 14px;
            width: 262px;
            background: rgba(240, 176, 0, 0.4);
          }
        }
        &-name,
        &-shop {
          white-space: nowrap;
          font-size: 52px;
          font-weight: 400;
          line-height: 73px;
          color: #000000;
        }
        &-place {
          white-space: nowrap;
          font-size: 24px;
          font-weight: 500;
          line-height: 40px;
          color: #000000;
        }
        &-msg {
          width: 70%;
          font-size: 20px;
          font-weight: 400;
          line-height: 34px;
          color: #999999;
          margin: 28px 0;
        }
      }
    }
  }
  &__page3 {
    border: 1px solid red;
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
            top: 52px;
            left: 10.5vw;
            height: 14px;
            width: 370px;
            background: rgba(240, 176, 0, 0.4);
          }
        }
        &-name,
        &-shop {
          white-space: nowrap;
          font-size: 52px;
          font-weight: 400;
          line-height: 73px;
          color: #000000;
        }
        &-place {
          white-space: nowrap;
          font-size: 24px;
          font-weight: 500;
          line-height: 40px;
          color: #000000;
        }
        &-msg {
          width: 70%;
          font-size: 20px;
          font-weight: 400;
          line-height: 34px;
          color: #999999;
          margin: 28px 0;
        }
      }
    }
  }
  &__page4 {
    height: 100vh;
    border: 1px solid red;
    &-head {
      text-align: center;
      margin-top: 10vh;
      &__name {
        font-size: 52px;
        line-height: 78px;
        color: #000000;
        span::after {
          content: "";
          position: absolute;
          top: 52px;
          left: 40%;
          height: 14px;
          width: 420px;
          background: rgba(240, 176, 0, 0.4);
        }
      }
      &__info {
        font-size: 30px;
        line-height: 40px;
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
        width: 320px;
        height: 319px;
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
            height: 80px;
            width: 80px;
            border-radius: 50%;
          }
        }
        &-name {
          margin-top: 32px;
          font-size: 24px;
          line-height: 29px;
          color: #000000;
          opacity: 1;
        }
        &-info {
          margin-top: 16px;
          font-size: 18px;
          line-height: 32px;
          color: #999999;
          opacity: 1;
        }
      }
      &__box:not(:first-child) {
        margin-left: 30px;
      }
    }
  }
  &__page5 {
    height: 100vh;
    border: 1px solid red;
    padding: 4% 4%;
    &-head {
      &__name {
        font-size: 52px;
        font-weight: 600;
        line-height: 78px;
        color: #000000;
        opacity: 1;
      }
      &__info {
        font-size: 30px;
        line-height: 40px;
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
        width: 380px;
        height: 430px;
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
        margin-left: 30px;
      }
    }
  }
  // &__page6 {
  //   height: 100vh;
  // }
}
</style>
