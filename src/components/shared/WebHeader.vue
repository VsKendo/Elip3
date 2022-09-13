<template>
  <div>
    <el-menu mode="horizontal" :ellipsis="false">
      <el-menu-item index="0">ELIP3 Website</el-menu-item>
      <div class="flex-grow" />
      <el-sub-menu index="1">
        <template #title>Links</template>
        <el-menu-item index="1-1">
          <el-link
            target="_blank"
            href="https://translate.google.com/"
            :underline="false"
          >
            <el-icon>
              <ChatLineSquare />
            </el-icon>
            Translator
          </el-link>
        </el-menu-item>
        <el-sub-menu index="1-2">
          <template #title>Dictionary</template>
          <el-menu-item index="1-2-1" class="el-sub-sub-menu">
            <el-link
              target="_blank"
              href="https://dictionary.cambridge.org/"
              :underline="false"
            >
              Cambridge
            </el-link>
          </el-menu-item>
          <el-menu-item index="1-2-2" class="el-sub-sub-menu">
            <el-link
              target="_blank"
              href="https://www.collinsdictionary.com/"
              :underline="false"
            >
              Collins
            </el-link>
          </el-menu-item>
        </el-sub-menu>
      </el-sub-menu>
    </el-menu>
  </div>
</template>

<script lang="ts" setup>
import { ChatLineSquare } from '@element-plus/icons'

// const handleSelect = (key: string, keyPath: string[]) => {
//   console.log(key, keyPath)
// }
</script>
<style>
.flex-grow {
  flex-grow: 1;
}

.el-menu--popup {
  min-width: 120px !important;
}

.el-sub-sub-menu {
  min-width: 100px !important;
  text-align: center;
  justify-content: center;
}
</style>
