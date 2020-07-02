<template>
  <div id="app">
    <mainHeader></mainHeader>
    <HTlogo></HTlogo>
<!--    <back_particles></back_particles>-->
  </div>
</template>

<script>
  import back_particles from "common/back_particles";
  import HTlogo from "components/common/HTlogo";
  import mainHeader from "components/content/mainHeader";
  import "particles.js"
  export default {
    name: 'APP',
    components: {
      back_particles,
      mainHeader,
      HTlogo
    }
  }

</script>
<style scoped>
  @import "assets/CSS/base.css";

</style>
