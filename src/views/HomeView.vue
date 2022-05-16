<template>
  <div>
    <el-container>
      <el-header class="header align-center">
        <div class="headerTitle align-center">
          <img src="@/assets/imgs/list.png">
          现代学徒云平台
        </div>
        <div class="headerState align-center">
          <span>武汉市</span>
          <span>2022/05/16</span>
          <span>16:25</span>
          <span>星期三</span>
          <span>21~22°C</span>
          <span>晴</span>
          <span>风力:112级</span>
          <span>风向:狂风骤雨</span>
        </div>
        <div class="headerUser align-center">
          <img src="@/assets/imgs/HeadPortrait.png">
          <span>hi!陌生人</span>
        </div>
        <div class="headerButton align-center">
          <img src="@/assets/imgs/switch.png">
          <span>退出</span>
        </div>
      </el-header>
      <el-container>
        <el-aside width="200px" class="aside">
          <el-col :span="12">
            <el-menu default-active="2" class="el-menu-vertical-demo" @open="handleOpen" @close="handleClose" background-color="#545c64" text-color="#fff" active-text-color="#ffd04b">
              <el-submenu index="1">
                <template slot="title">
                  <i class="el-icon-location"></i>
                  <span>导航一</span>
                </template>
                <el-menu-item-group>
                  <template slot="title">分组一</template>
                  <el-menu-item index="1-1">选项1</el-menu-item>
                  <el-menu-item index="1-2">选项2</el-menu-item>
                </el-menu-item-group>
                <el-menu-item-group title="分组2">
                  <el-menu-item index="1-3">选项3</el-menu-item>
                </el-menu-item-group>
                <el-submenu index="1-4">
                  <template slot="title">选项4</template>
                  <el-menu-item index="1-4-1">选项1</el-menu-item>
                </el-submenu>
              </el-submenu>
              <el-menu-item index="2">
                <i class="el-icon-menu"></i>
                <span slot="title">导航二</span>
              </el-menu-item>
              <el-menu-item index="3" disabled>
                <i class="el-icon-document"></i>
                <span slot="title">导航三</span>
              </el-menu-item>
              <el-menu-item index="4">
                <i class="el-icon-setting"></i>
                <span slot="title">导航四</span>
              </el-menu-item>
            </el-menu>
          </el-col>
        </el-aside>
        <el-main class="main">Main</el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.header {
  padding: 0 20px;
  background: #1888d0;
  color: #fff;
  & .headerTitle {
    gap: 20px;
    flex: 15;
    & img {
      width: 20px;
    }
  }
  & .headerState {
    flex: 5;
    gap: 0px 10px;
    & span {
      font-size: 10px;
    }
  }
  & .headerUser {
    flex: 2;
    gap: 0px 10px;
    & img {
      padding-left: 25px;
      width: 50px;
    }
  }
  & .headerButton {
    & img {
      width: 30px;
    }
  }
}
.aside {
  height: calc(100vh - 50px);
}
.main {
  background: #92e1c7;
}
</style>