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
import Title from "./title/title";
import {skillData} from "../mock/skill.js"
export default {
  data () {
    return {
      itemData:skillData
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