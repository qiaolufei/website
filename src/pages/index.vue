<template>
  <div class="index">
    <page1></page1>
    <page2></page2>
    <page3></page3>
    <page4></page4>
    <page5></page5>
    <page6></page6>
  </div>
</template>
<script>
import page1 from '@/components/page1'
import page2 from '@/components/page2'
import page3 from '@/components/page3'
import page4 from '@/components/page4'
import page5 from '@/components/page5'
import page6 from '@/components/page6'
export default {
  components: {
    page1, page2, page3, page4, page5, page6
  }
}
</script>
<style lang="less">
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
  overflow-x: hidden
}
</style>
