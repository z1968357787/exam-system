<template>
  <div class="hello">
    <el-container style=" border: 1px solid #eee">
      <el-aside width="300px" style="background-color: rgba(91,209,215,1)">
        <el-menu :default-openeds="['1', '3']">
          <el-submenu index="1">
            <template slot="title"><i class="el-icon-message"></i>试题库管理</template>
            <!--<el-submenu index="1-4">-->
              <!--<template slot="title">选项4</template>-->
              <el-menu-item index="1-1">试题添加</el-menu-item>
            <!--</el-submenu>-->
          </el-submenu>
          <el-submenu index="2">
            <template slot="title"><i class="el-icon-menu"></i>笔试模块管理</template>
            <el-submenu index="2-1">
              <template slot="title">行政能力模块</template>
              <el-menu-item index="2-1-1">基础能力训练</el-menu-item>
              <el-menu-item index="2-1-2">分类训练</el-menu-item>
              <el-menu-item index="2-1-3">限时训练</el-menu-item>
              <el-menu-item index="2-1-4">模拟测试</el-menu-item>
            </el-submenu>
            <el-submenu index="2-2">
              <template slot="title">申论能力模块</template>
              <el-menu-item index="2-2-1">基础能力训练</el-menu-item>
              <el-menu-item index="2-2-2">分类训练</el-menu-item>
              <el-menu-item index="2-2-3">限时训练</el-menu-item>
              <el-menu-item index="2-2-4">限字训练</el-menu-item>
              <el-menu-item index="2-2-5">模拟测试</el-menu-item>
            </el-submenu>
          </el-submenu>
          <el-submenu index="3">
            <template slot="title"><i class="el-icon-setting"></i>面试模块管理</template>
            <el-submenu index="3-1">
              <template slot="title">面试基础能力</template>
              <el-menu-item index="3-1-1">基础要素能力测试</el-menu-item>
              <el-menu-item index="3-1-2">面试细节测试与训练</el-menu-item>
              <el-menu-item index="3-1-3">听题能力测试与训练</el-menu-item>
              <el-menu-item index="3-1-4">思考习惯测试与训练</el-menu-item>
              <el-menu-item index="3-1-5">语言能力和技巧测试与训练</el-menu-item>
              <el-menu-item index="3-1-6">答题声音检测</el-menu-item>
            </el-submenu>
            <el-submenu index="3-2">
              <template slot="title">结构化面试</template>
              <el-menu-item index="3-2-1">基础要素能力</el-menu-item>
              <el-menu-item index="3-2-2">综合分析能力</el-menu-item>
              <el-menu-item index="3-2-3">计划组织协调能力</el-menu-item>
              <el-menu-item index="3-2-4">解决实际问题能力</el-menu-item>
              <el-menu-item index="3-2-5">模拟测试</el-menu-item>
              <el-menu-item index="3-2-5">应变能力</el-menu-item>
              <el-menu-item index="3-2-5">人际沟通能力</el-menu-item>
              <el-menu-item index="3-2-5">模拟测试</el-menu-item>
              <el-menu-item index="3-2-5">实时打分</el-menu-item>
            </el-submenu>
            <el-submenu index="3-3">
              <template slot="title">无领导小组讨论</template>
              <el-menu-item index="3-3-1">基础要素能力</el-menu-item>
              <el-menu-item index="3-3-2">模拟测试</el-menu-item>
              <el-menu-item index="3-3-3">实时打分</el-menu-item>
            </el-submenu>
          </el-submenu>
          <el-submenu index="4">
            <template slot="title"><i class="el-icon-setting"></i>基础能力提升</template>
            <el-menu-item index="4-1">好文章读背、赏析与分享</el-menu-item>
            <el-menu-item index="4-2">名人名句读背</el-menu-item>
            <el-menu-item index="4-3">焦点和热点新闻社评</el-menu-item>
            <el-menu-item index="4-4">思维方法学习</el-menu-item>
            <el-menu-item index="4-5">学习成果测试</el-menu-item>
            <el-menu-item index="4-6">线上视频辅导和答疑</el-menu-item>
            <el-menu-item index="4-7">心得体会分享</el-menu-item>
            <el-menu-item index="4-8">分享查阅</el-menu-item>
          </el-submenu>
          <el-submenu index="5">
            <template slot="title"><i class="el-icon-setting"></i>五、用户管理模块</template>
            <el-menu-item index="5-1">基础数据收集</el-menu-item>
            <el-menu-item index="5-2">课程推送</el-menu-item>
            <el-menu-item index="5-3">用户推荐统计</el-menu-item>
            <el-menu-item index="5-4">使用反馈</el-menu-item>
            <el-menu-item index="5-5">发送节日问候</el-menu-item>
          </el-submenu>
        </el-menu>
      </el-aside>

      <el-container>
        <el-header style="text-align: right; font-size: 12px">
          <el-dropdown>
            <i class="el-icon-setting" style="margin-right: 15px"></i>
            <el-dropdown-menu slot="dropdown">
              <el-dropdown-item>查看</el-dropdown-item>
              <el-dropdown-item>新增</el-dropdown-item>
              <el-dropdown-item>删除</el-dropdown-item>
            </el-dropdown-menu>
          </el-dropdown>
          <span>王小虎</span>
        </el-header>
        <!--
        <el-main>
          <el-table :data="tableData">
            <el-table-column prop="date" label="日期" width="140">
            </el-table-column>
            <el-table-column prop="name" label="姓名" width="120">
            </el-table-column>
            <el-table-column prop="address" label="地址">
            </el-table-column>
          </el-table>
        </el-main>-->
      </el-container>
    </el-container>

<!--
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <ul>
      <li>
        <a
          href="https://vuejs.org"
          target="_blank"
        >
          Core Docs
        </a>
      </li>
      <li>
        <a
          href="https://forum.vuejs.org"
          target="_blank"
        >
          Forum
        </a>
      </li>
      <li>
        <a
          href="https://chat.vuejs.org"
          target="_blank"
        >
          Community Chat
        </a>
      </li>
      <li>
        <a
          href="https://twitter.com/vuejs"
          target="_blank"
        >
          Twitter
        </a>
      </li>
      <br>
      <li>
        <a
          href="http://vuejs-templates.github.io/webpack/"
          target="_blank"
        >
          Docs for This Template
        </a>
      </li>
    </ul>
    <h2>Ecosystem</h2>
    <ul>
      <li>
        <a
          href="http://router.vuejs.org/"
          target="_blank"
        >
          vue-router
        </a>
      </li>
      <li>
        <a
          href="http://vuex.vuejs.org/"
          target="_blank"
        >
          vuex
        </a>
      </li>
      <li>
        <a
          href="http://vue-loader.vuejs.org/"
          target="_blank"
        >
          vue-loader
        </a>
      </li>
      <li>
        <a
          href="https://github.com/vuejs/awesome-vue"
          target="_blank"
        >
          awesome-vue
        </a>
      </li>
    </ul>-->
  </div>
</template>

<style>
.el-header {
  background-color: #B3C0D1;
  color: #333;
  line-height: 60px;
}

.el-aside {
  color: #333;
}
</style>

<script>
export default {
  name: 'HelloWorld',
  data() {
    const item = {
      date: '2016-05-02',
      name: '王小虎',
      address: '上海市普陀区金沙江路 1518 弄'
    };
    return {
      tableData: Array(20).fill(item)
    }
  }
};
</script>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
