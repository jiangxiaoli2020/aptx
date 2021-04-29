<template>
    <div id="loginWrapper">
    <div id="loginContentBody">
      <el-card class="box-card">
        <div slot="header" class="clearfix">
          <span>卡片名称</span>
          <el-button style="float:right;padding: 3px 0" type="text">忘记密码</el-button>
        </div>
        <div id="loginContentBody">
        <el-input id="username" v-model="user.username" clearable></el-input>
        <el-input id="password" v-model="user.password" clearable></el-input>
    </div>
   <div id="loginSubmit">
     <el-button id="systemSubmit">
       <el-button id="systemSubmit">登录</el-button>
   </div>
      </el-card>
    </div>
    </div>
            
</template>

<script>
export default {
  data(){
    return{
      user:{
        username:"",
        password:""
      }
    }
  }
};
</script>

 
<style>
#loginWrapper {
  background-color: purple;
  height: 100%;
}
#loginContent {
  width: 400px;
  margin: 0 auto;
  padding-top: 100px;
}
#systemSubmit {
  display: block;
  margin: 0 auto;
  background-color: seashell;
  color: white;
}
</style>
