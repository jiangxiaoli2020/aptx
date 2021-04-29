<template>
  <div id="headerWrapper">
    <div id="headerTitle">
      <span>{{ message }}</span>
    </div>
    <div id="headerFuction">
      <router-link to="/login">
        <el-button>系统登录</el-button>
      </router-link>

      <router-link to="/work">
        <el-button>工作信息</el-button>
      </router-link>

      <router-link to="/reader">
        <el-button>读者信息</el-button>
      </router-link>

      <router-link to="/book">
        <el-button>图书信息</el-button>
      </router-link>
      <router-link to="/cnnode">
        <el-button>node论坛</el-button>
      </router-link>
    </div>
  </div>
</template>
 


<style>
#headerTitle {
  display: inline-block;
  height: 60px;
  background-color: blue;
  font-size: 20px;
  font-weight: bolder;
}
#headerFunction {
  display: inline-block;
  float: right;
  margin-top: 10px;
}
#headerFunction > a > .el-button {
  background-color: rgb(101, 28, 236);
  color: honeydew;
  border-color: olive;
  margin-left: 5px;
}
</style>