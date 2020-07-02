<template>
  <div id="header">
    <headers></headers>
    <siderTab></siderTab>
  </div>
</template>

<script>
import headers from "components/common/headers"
import siderTab from "components/common/sider-tab"
export default {
  name: "mainHeader",
  components: {
    headers,
    siderTab
  }
}
</script>

<style scoped>

</style>
