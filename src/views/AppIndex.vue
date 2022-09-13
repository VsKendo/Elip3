<template>
  <div>
    <el-container>
      <!--      <el-aside width="200px">Aside</el-aside>-->
      <el-container>
        <el-header style="">
          <WebHeader />
        </el-header>
        <el-container>
          <side-bar />
          <el-container>
            <el-main>main</el-main>
            <Webfooter/>
<!--            <el-footer>Footer</el-footer>-->
          </el-container>
        </el-container>
      </el-container>
    </el-container>
  </div>
</template>
<script lang="ts" setup>
import SideBar from '@/components/shared/SideBar'
import WebHeader from '@/components/shared/WebHeader'
import Webfooter from '@/components/shared/WebFooter'
</script>
