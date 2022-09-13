<template>
  <el-menu
    style="height: 90vh; width: 15%"
    default-active="1"
    class="el-menu-vertical-demo"
    @open="handleOpen"
    @close="handleClose"
  >
    <el-menu-item index="1">
      <el-icon>
        <icon-menu />
      </el-icon>
      <span>index</span>
    </el-menu-item>
    <el-sub-menu index="2">
      <template #title>
        <el-icon>
          <icon-location />
        </el-icon>
        <span>Vocabulary Targets</span>
      </template>
      <el-menu-item-group title="Weekly">
        <el-menu-item index="1-1">Week 1</el-menu-item>
        <el-menu-item index="1-2">Week 2</el-menu-item>
      </el-menu-item-group>
      <el-menu-item-group title="Others">
        <el-menu-item index="1-3" disabled>Nothing Here</el-menu-item>
      </el-menu-item-group>
    </el-sub-menu>
    <el-menu-item index="3">
      <el-icon>
        <setting />
      </el-icon>
      <span>About</span>
    </el-menu-item>
  </el-menu>
</template>

<script lang="ts" setup>
import {
  Menu as IconMenu,
  Location as IconLocation,
  Setting
} from '@element-plus/icons-vue'

const handleOpen = (key: string, keyPath: string[]) => {
  console.log(key, keyPath)
}
const handleClose = (key: string, keyPath: string[]) => {
  console.log(key, keyPath)
}
</script>
