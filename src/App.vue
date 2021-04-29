<template>
  <div id="app">
    <!--3.使用子组件-->
    <el-container>
      <el-header id="headerBook">
        <Header />
      </el-header>

      <el-main id="mainBook">
        <!--<Login />-->
        <router-view></router-view>
      </el-main>
      <el-footer id="footerBook">
        <Footer />
      </el-footer>
    </el-container>
  </div>
</template>

<script>
import FooterVue from "./components/Footer";
//1.导入Header 子组件
import Header from "./components/Header";
import Login from "./components/Login";
import Footer from "./components/Footer";
//2.注册 子组件
export default {
  name: "App",
  components: {
    Header,
    Login,
    Footer,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
