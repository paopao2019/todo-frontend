<template>
  <el-container>
    <el-header>gin gorm 框架小练习</el-header>
    <el-main>
      <el-row type="flex" justify="center">
        <el-col :xs="20" :span="12" >
          <div class="grid-content">
            <el-divider>
              <h1>TODO 清单</h1>
            </el-divider>
            <TodoList></TodoList>
          </div>
        </el-col>
      </el-row>
    </el-main>
    <install-tip> </install-tip>
    <el-footer>代码原始来源七米: <a href="https://github.com/Q1mi/bubble_frontend">七米源码</a></el-footer>
  </el-container>


</template>

<script>
// @ is an alias to /src
import TodoList from "@/components/TodoList.vue";
import InstallTip from "../components/InstallTip";

export default {
  name: "Index",
  components: {
    TodoList,
    InstallTip
  }
};
</script>
<style>
.el-header,
.el-footer {
  background-color: #409eff;
  color: #fff;
  text-align: center;
  line-height: 60px;
}
.el-footer {
  background-color: #909399;
  /*display: block;*/
  /*width: 100%;*/
  /*position: fixed;*/
  /*bottom: 0px;*/

}
</style>