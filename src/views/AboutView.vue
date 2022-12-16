<template>
  <span>Message: {{ "base"
      ? `var(--el-border-radius-"base")`
      : ''
  }}</span>
  <div class="radius1">
    <!-- header -->
    <div class="page_header">
      <img alt="paper plane" src="../assets/icon-paper-plane.png">
      <p class="header_text">Vue Login Page Demo</p>
    </div>

    <!-- left content -->
    <div class="intro">
      <p>Login Title</p>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue'

</script>
<style scoped>
.radius1 {
  height: 600px;
  width: 1200px;
  border: 1px solid var(--el-border-color);
  border-radius: 50px;
  /* background-color:aqua; */

  background: linear-gradient(to right, #0229bf 0%, #0229bf 50%, white 50%, white 100%);
  fill: rgb(8, 8, 8);
  /* box-shadow: var(--el-box-shadow-dark), */
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.12), 0 0 6px rgba(0, 0, 0, 0.04);
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  margin: auto;
  /* boxShadow: 'var(--el-box-shadow-dark)', */
}

.page_header {
  position: relative;
  top: 22px;
  left: -533px;
}
.header_text {
  font-size: 16pt;
  position: relative;
  left: 120px;
  top: -37px;
  color:white;
  font-family:"Lucida Sans Unicode", "Lucida Grande", sans-serif;
}

.intro {
  position: relative;
  left: -533px;
  margin-top: 100;
  /* padding-top: 200; */
}
</style>
