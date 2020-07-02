<template>
  <div class="sider_tab">
    <div class="item">首页</div>
    <div class="item">关于我</div>
    <div class="item">赞赏•支持</div>
  </div>
</template>

<script>
export default {
  name: "sider-tab"
}
</script>

<style scoped>
  .sider_tab {
    display: flex;
    flex-direction: column;
    justify-content: space-between;

    width: 100px;
    height: 100px;
    font-family: "冬青黑体简体中文 W3";
    font-size: 18px;
    font-weight: 600;
    position: absolute;
    left: 16%;
    top: 20%;

    cursor: pointer;
  }
  .item {
    flex: 1;
  }
</style>
