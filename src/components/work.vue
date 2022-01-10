<!--  -->
<template>
  <div class="workWrapper">
    <Title titleName="工作经历"/>
    <div class="workItemWrapper"> 
      <div class="workItem">
        <div>
          <svg class="icon" aria-hidden="true">
            <use xlink:href="#icon-icradioture"></use>
          </svg>
          <span class="workDate">2017-07 - 至今</span>
        </div>
        <div class="center">北京某科技有限公司</div>
        <div class="right">前端工程师</div>
      </div>
      <!-- 工作内容 -->
      <ul>
        <li v-for="(item,index) in itemData" :key="index">
          <span class="dot"></span>
          {{item}}
        </li>
      </ul>

    </div>
  </div>
</template>

<script>
import Title from "./title/title"
export default {
  data () {
    return {
      itemData:[
        "参与智慧教育综合服务平台的研发及维护工作",
        "负责协同Java、PHP、Python等后端进行业务流程梳理及接口联调",
        "负责对接科大讯飞、百度智慧教育平台、腾讯RTC等平台API研发智能作文录入批改、在线课堂",
        "负责针对不同维度的数据进行数据可视化开发",
        "主导项目模块拆分，降低项目的复杂度",
        "参与电商小程序及电商后台管理系统的研发",
        "负责协同后端人员对接微信小程序直播、小程序支付、产品扫描录入"
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
.workWrapper{
  margin-top: 32px;
}
.workItemWrapper{
  margin-top: 16px;
}
.workItem{
  display: flex;
  justify-content: space-between;
}
.workItem>div{
  flex: 1;
  text-align: left;
}
.workDate{
  margin-left: 9px;
}
.center{
  text-align: center !important;
}
.right{
  text-align: right !important;
}
ul{
  list-style: none;
  margin-top: 20px;
  margin-left: 20px;
}
ul li{
  text-align: left;
  margin-bottom: 10px;
}
li span{
  margin-left: 10px;
  display: inline-block;
}
.dot{
  display: inline-block;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: #0072bd;
  margin-right: 8px;
}

</style>