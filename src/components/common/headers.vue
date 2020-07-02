<template>
  <div id="nav_bar">
<!--    <el-tabs v-model="activeName" @tab-click="handleClick">-->
<!--      <el-tab-pane label="首页" name="first">首页</el-tab-pane>-->
<!--      <el-tab-pane label="学习" name="second">学习</el-tab-pane>-->
<!--      <el-tab-pane label="作品" name="third">作品</el-tab-pane>-->
<!--      <el-tab-pane label="牢骚" name="fourth">牢骚</el-tab-pane>-->
<!--      <el-tab-pane label="联系我" name="fivth">联系我</el-tab-pane>-->
<!--      <el-tab-pane label="玩一玩" name="sixth">玩一玩</el-tab-pane>-->
<!--    </el-tabs>-->
    <div @click="get_nav_list">
      <button class="menu" onclick="this.classList.toggle('opened');this.setAttribute('aria-expanded', this.classList.contains('opened'))" aria-label="Main Menu">
        <svg width="44" height="44" viewBox="0 0 100 100">
          <path class="line line1" d="M 20,29.000046 H 80.000231 C 80.000231,29.000046 94.498839,28.817352 94.532987,66.711331 94.543142,77.980673 90.966081,81.670246 85.259173,81.668997 79.552261,81.667751 75.000211,74.999942 75.000211,74.999942 L 25.000021,25.000058" />
          <path class="line line2" d="M 20,50 H 80" />
          <path class="line line3" d="M 20,70.999954 H 80.000231 C 80.000231,70.999954 94.498839,71.182648 94.532987,33.288669 94.543142,22.019327 90.966081,18.329754 85.259173,18.331003 79.552261,18.332249 75.000211,25.000058 75.000211,25.000058 L 25.000021,74.999942" />
        </svg>
      </button>
    </div>
    <div class="mask">
    </div>
  </div>
</template>

<script>
  export default {
    name: "headers",
    data () {
      return {
        navList: ["首页", "学习", "作品", "牢骚", "联系我", "玩一玩"]
      }
    },
    methods: {
      get_nav_list () {

      }
    },
    components: {
    }
  }
</script>

<style scoped>
  .menu {
    background-color: transparent;
    border: none;
    cursor: pointer;
    display: flex;
    padding: 0;
  }
  .line {
    fill: none;
    stroke: black;
    stroke-width: 2;
    transition: stroke-dasharray 600ms cubic-bezier(0.4, 0, 0.2, 1),
    stroke-dashoffset 600ms cubic-bezier(0.4, 0, 0.2, 1);
  }
  .line1 {
    stroke-dasharray: 60 207;
    stroke-width: 6;
  }
  .line2 {
    stroke-dasharray: 60 60;
    stroke-width: 6;
  }
  .line3 {
    stroke-dasharray: 60 207;
    stroke-width: 6;
  }
  .opened .line1 {
    stroke-dasharray: 90 207;
    stroke-dashoffset: -134;
    stroke-width: 6;
  }
  .opened .line2 {
    stroke-dasharray: 1 60;
    stroke-dashoffset: -30;
    stroke-width: 6;
  }
  .opened .line3 {
    stroke-dasharray: 90 207;
    stroke-dashoffset: -134;
    stroke-width: 6;
  }
  .mask {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background: #3c3c3c;
    opacity: .8;
  }
</style>