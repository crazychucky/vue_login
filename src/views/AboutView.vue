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
    <!-- <div class="intro">
      <p class="intro_title">Login Title</p>
      <p class="intro_text">This is login context:The quick brown fox jumps over the lazy dog,The quick brown fox jumps over the lazy dog,The quick brown fox jumps over the lazy dog.</p>
      <img alt="login" src="../assets/email.png" class="intro_img">
    </div> -->

    <div class="main_container">OK</div>
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
  width:600px;
  position: relative;
  margin-top: 100;
  /* padding-top: 200; */
}

.intro_title {
  font-size: 32pt;
  color:white;
  text-indent:55px;
  text-align:left;
  /* background-color:red; */
  font-family:"Lucida Sans Unicode", "Lucida Grande", sans-serif;
}
.intro_text {
  position: relative;
  left: 40px;

  width:520px;
  font-size: 12pt;
  color:white;
  /* background-color:red; */
  text-align:left;
  text-indent:25px;
  font-family:"Lucida Sans Unicode", "Lucida Grande", sans-serif;
  z-index: 5;   /*置于底层*/
}
.intro_img {
  width:255px;
  height: 255px;
  position: relative;
  top: -68px;
  z-index: 1;  /*置于底层*/
}

.main_container {
  width:1200;
  height: 200;
  background-color:red
}
</style>
