<template>
  <div id="app">
    <headers></headers>
<!--    <back_particles></back_particles>-->
  </div>
</template>

<script>
  import back_particles from "./components/common/back_particles";
  import headers from "./components/common/headers";
  import "particles.js"
  export default {
    name: 'APP',
    components: {
      back_particles,
      headers
    }
  }

</script>
<style scoped>
</style>
