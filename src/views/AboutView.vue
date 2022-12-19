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

    <div class="main_container">
      <!-- <div class="div-inline">第一个div盒子</div>
      <div class="div-inline">第二个盒子</div>
      <div class="div-inline">第三个盒子</div> -->
      <div class="intro">
        <p class="intro_title">Intro Title</p>
        <p class="intro_text">This is login context:The quick brown fox jumps over the lazy dog,The quick brown fox jumps over the lazy dog,The quick brown fox jumps over the lazy dog.</p>
        <img alt="login" src="../assets/email.png" class="intro_img">
      </div>
      <div class="login">
        <p class="login_title">Login</p>
        <div>
          <el-input v-model="input_name" placeholder="Please input" size="large" :prefix-icon="User" class="name_input"></el-input>
        </div>
        <div>
          <el-input v-model="input_pass" type="password" placeholder="Please input password" show-password size="large" :prefix-icon="Lock" class="password_input"></el-input>
        </div>
        <div>
          <el-checkbox v-model="check_save_name" size="small" class="save_checker">Remember me</el-checkbox>
          <el-button  type="info" link size="small" class="forget_pass">Forget Password?</el-button> 
        </div>

        <div>
          <el-button type="primary" round class="login_btn">LOGIN</el-button>
          <!-- <el-button type="primary" :icon="Search">Search</el-button> -->
        </div>
        <!-- TODO:input name password -->
        <!-- <p class="intro_text">This is login context:The quick brown fox jumps over the lazy dog,The quick brown fox jumps over the lazy dog,The quick brown fox jumps over the lazy dog.</p> -->
        <!-- <img alt="login" src="../assets/email.png" class="intro_img"> -->
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue'
import { User,Lock } from '@element-plus/icons-vue'
const input_name = ref('')
const input_pass = ref('')
const check_save_name = ref(true)

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
  /* border: 3px solid #73AD21; */
  /* position: relative; */
  margin-top: 100;
  float:left;
  /* padding-top: 200; */
}
.intro1 {
  width:600px;
  /* border: 3px solid #73AD21; */
  /* position: relative; */
  margin-top: 100;
  /* display:inline; */
  float:right;
  background-color:white;
  /* padding-top: 200; */
}

.intro_title {
  font-size: 32pt;
  width:600px;
  color:white;
  text-indent:55px;
  text-align:left;
  /* background-color:red; */
  font-family:"Lucida Sans Unicode", "Lucida Grande", sans-serif;
}
.intro_text {
  position: relative;
  left: 46px;

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

.login {
  width:600px;
  /* border: 3px solid #73AD21; */
  /* position: relative; */
  margin-top: 100;
  /* display:inline; */
  float:right;
  /* background-color:blueviolet; */
}

.login_title {
  font-size: 32pt;
  width:600px;
  color:#0229bf;
  text-align:center;
  /* background-color:red; */
  font-family:"Lucida Sans Unicode", "Lucida Grande", sans-serif;
}

.main_container {
  width:1200;
  height: 500;
}
.name_input {
  width:300px;
}
.password_input {
  padding-top: 15px;
  padding-bottom: 3px;
  width:300px;
}

.save_checker {
  position: absolute;
  left: 750px;
}
.forget_pass {
  position: absolute;
  right: 150px;
}
.test_debug {
  background-color:plum;
}
.login_btn {
  margin-top: 38px;
  width:260px;
  height:40px;
  background-color:blue;
}
</style>
