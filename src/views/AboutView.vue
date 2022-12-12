<template>
  <span>Message: {{"base"
            ? `var(--el-border-radius-"base")`
            : ''}}</span>
   <div
        class="radius1"
    />
</template>

<script lang="ts" setup>
import { ref } from 'vue'

</script>
<style scoped>
.radius1 {
  height: 400px;
  width: 800px;
  border: 1px solid var(--el-border-color);
  border-radius: 50px;
  margin-top: 20px;
  background-color:aqua;
  fill:rgb(8, 8, 8);
  /* box-shadow: var(--el-box-shadow-dark), */
  box-shadow: 0 2px 4px rgba(0,0,0,0.12),0 0 6px rgba(0,0,0,0.04)
  /* boxShadow: 'var(--el-box-shadow-dark)', */
}
</style>
