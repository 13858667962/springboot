<template>
  <div>
    <el-menu
        style="width: 200px;min-height: calc(100vh - 50px)"
        default-active="user" router
        class="el-menu-vertical-demo"
        @open="handleOpen"
        @close="handleClose"
    >
      <el-sub-menu index="1">
        <template #title>
          <i class="el-icon-location"></i>
          <span>系统管理</span>
        </template>
          <el-menu-item index="user">用户管理</el-menu-item>
          <el-menu-item index="data">数据管理</el-menu-item>
      </el-sub-menu>

    </el-menu>

  </div>
</template>

<script>
import {Location,Document,Setting} from "@element-plus/icons";
import {Menu} from "@element-plus/icons-vue"

export default {
  name: "Aside",
  components:{
    Location,
    Menu,
    Document,
    Setting
  },
}
</script>

<style scoped>

</style>