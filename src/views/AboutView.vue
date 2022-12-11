<template>
  <span>Message: {{"base"
            ? `var(--el-border-radius-"base")`
            : ''}}</span>
   <div
        class="radius1"
        :style="{
          borderRadius: 'var(--el-border-radius-round)',
        }"
      />
</template>

<script lang="ts" setup>
import { ref } from 'vue'

</script>
<style scoped>
.radius1 {
  height: 400px;
  width: 50%;
  border: 2px solid var(--el-border-color);
  margin-top: 20px;
  /* box-shadow: var(--el-box-shadow-dark), */
  box-shadow: 0 2px 4px rgba(0,0,0,0.12),0 0 6px rgba(0,0,0,0.04)
  /* boxShadow: 'var(--el-box-shadow-dark)', */
}
</style>
