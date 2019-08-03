<template>
  <el-container>
    <el-header>
      <img
        src="../assets/header.png"
        alt=""
      >
      <img
        class="toubu"
        src="../assets/toubu.png"
        alt=""
      >
    </el-header>
    <el-container
      class="container2"
      width="1206px"
    >
      <el-aside width="218px">
        <img
          class="one"
          src="../assets/avatarbgc.png"
          alt=""
        >
        <img
          class="touxiang"
          src="../assets/avatar.png"
          alt=""
        >
        <div class="word">
          <p>Admin</p>
          <p>2021级</p>
        </div>
        <el-menu
          default-active="1"
          class="el-menu-vertical-demo"
          @open="handleOpen"
          @close="handleClose"
        >
          <el-submenu index="1">
            <template slot="title">
              <i class="el-icon-s-custom"></i>
              <span>用户中心</span>
            </template>
          </el-submenu>
          <el-menu-item index="2">
            <i class="el-icon-menu"></i>
            <span slot="title">测评中心</span>
          </el-menu-item>
          <el-menu-item index="3">
            <i class="el-icon-video-camera-solid"></i>
            <span slot="title">课程中心</span>
          </el-menu-item>
          <el-menu-item index="4">
            <i class="el-icon-setting"></i>
            <span slot="title">任务中心</span>
          </el-menu-item>
          <el-menu-item index="5">
            <i class="el-icon-document"></i>
            <span slot="title">成长档案</span>
          </el-menu-item>
          <el-menu-item index="6">
            <i class="el-icon-setting"></i>
            <span slot="title">全球数据库</span>
          </el-menu-item>
        </el-menu>
      </el-aside>
      <el-main>Main</el-main>
    </el-container>
  </el-container>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'home',
  methods: {
    handleOpen (key, keyPath) {
      console.log(key, keyPath)
    },
    handleClose (key, keyPath) {
      console.log(key, keyPath)
    }
  }
}
</script>

<style scope lang="less">
.el-container {
  position: relative;
  height: 100%;
  .el-header {
    height: 60px;
    padding: 0px;
    width: 100%;
    position: relative;
    .toubu {
      position: absolute;
      top: 0;
    }
  }
  .touxiang {
    position: absolute;
    top: 40px;
    left: 60px;
  }
  .word {
    position: absolute;
    left: 60px;
    top: 110px;
    text-align: center;
    color: #fff;
  }
  .el-main {
    margin-left: 20px;
    background-color: #fff;
    border-radius: 20px;
  }
}
</style>
