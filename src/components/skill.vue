<!-- 技能情况 -->
<template>
  <div class="skillWrapper">
    <Title titleName="技能情况"></Title>
    <ul>
      <li v-for="(item,index) in itemData" :key="index">
        <svg class="icon" aria-hidden="true">
          <use xlink:href="#icon-fuxuankuang_xuanzhong"></use>
        </svg>
        <span>{{item}}</span>
      </li>
    </ul>
  </div>
</template>

<script>
import Title from "./title/title"
export default {
  data () {
    return {
      itemData:[
        "熟悉HTML CSS静态页面搭建及前端性能优化,高保真还原设计稿",
        "熟练掌握JavaScript ES6语法",
        "熟悉前后端分离技术，包括AJAX、webScoket、跨域、前端路由搭建、数据持久化",
        "熟悉Vue技术栈，包括 Vuecli、VueRouter、vuex、keep-alive、axois",
        "熟悉Vue3.0新特性，包括CompositionAPI的使用",
        "熟悉uniapp跨平台开发，打包安卓APP端、H5端、小程序端项目",
        "熟练掌握Echarts5.0数据可视化开发、LOCA数据可视化开发、uEcharts跨平台可视化开发",
        "熟练掌握ElementUI、AntDesign、uViewe、colorUI等UI框架",
        "了解React技术栈，包括ReactHooks、reactRouter",
        "了解Node.js基本语法和常用模块",
        "了解TypeScript基本用法"
      ]
    };
  },

  components:{
    Title
  },

  computed:{},

  mounted(){},

  methods:{}
}

</script>
<style scoped>
.skillWrapper{
  margin-top: 32px;
}
ul{
  list-style: none;
  margin-top: 20px;
}
ul li{
  text-align: left;
  margin-bottom: 10px;
}
li span{
  margin-left: 10px;
  display: inline-block;
}
</style>