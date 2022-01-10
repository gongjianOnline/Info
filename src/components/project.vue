<!-- 项目经验 -->
<template>
  <div class="projectWrapper">
    <Title titleName="项目经验"/>
    <div class="proWrapper" v-for="(item,index) in projectData" :key="index">
      <div class="proInfo">
        <div>
          <svg class="icon" aria-hidden="true">
            <use xlink:href="#icon-icradioture"></use>
          </svg>
          <span class="proTitle">{{item.projectName}}</span>
        </div>
        <div class="proManipulate">
          <span v-for="(visitItem,visitIndex) in item.visitList" :key="visitIndex">{{visitItem.name}}</span>
        </div>
      </div>
      <div class="proDescribe">
        背景： {{item.projectDescribe}}
      </div>
      <div class="proSkill">
        技术栈： {{item.skillArr}}
      </div>
      <div class="proItem">
        <div>负责部分</div>
        <ul>  
          <li v-for="(itemItem,itemIndex) in item.itemData" :key="itemIndex">
            <span class="dot"></span>
            {{itemItem}}
          </li>
        </ul>
      </div>
      <!-- 分割线 -->
      <hr>
    </div>
  </div>
</template>

<script>
import Title from "./title/title";
import {projectData} from "../mock/project.js"
export default {
  data () {
    return {
      projectData:projectData
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
.projectWrapper{
  margin-top: 32px;
}
.proWrapper{
  margin-top: 16px;
}
.proInfo{
  display: flex;
  justify-content: space-between;
  font-size: 18px;
}
.proInfo>div{
  flex: 1;
}
.proInfo:nth-child(1){
  text-align: left;
}
.proTitle{
  margin-left: 14px;
}
.proManipulate{
  text-align: right;
}
.proManipulate>span{
  margin-left: 10px;
  cursor: pointer;
}
/* 项目描述 */
.proDescribe,.proSkill{
  text-align: left;
  margin-top: 10px;
  font-size: 18px;
}
/* 负责部分 */
.proItem{
  text-align: left;
  margin-top: 10px;
}

ul{
  list-style: none;
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