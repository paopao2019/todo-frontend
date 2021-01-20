<template>
  <el-card class="box-card">
    <div slot="header" class="clearfix">
      <span>部署说明</span>
      <el-button style="float: right; padding: 3px 0" type="text">
        <a href="http://www.baidu.com" target="_blank">代码地址</a>
      </el-button>
    </div>
    <div class="text item">
      1. 前端安装依赖包 npm install
      <br>
      2. 前端启动 npm run serve <strong>注意:(调用后端修改 plugins中的axios.js 中的 baseURL配置)</strong>
      <br>
      3. 后端要注意跨域问题
    </div>
  </el-card>

</template>

<script>
  export default {
    name: "InstallTip"
  }
</script>

<style scoped>
  .text {
    font-size: 14px;
  }

  .item {
    margin-bottom: 18px;
  }

  .clearfix:before,
  .clearfix:after {
    display: table;
    content: "";
  }
  .clearfix:after {
    clear: both
  }

  .box-card {
    width: 300px;
    position: fixed;
    top: 50px;
    background-color: cyan;
  }
</style>