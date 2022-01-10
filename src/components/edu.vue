<!--  -->
<template>
  <div class="eduWrapper">
    <Title titleName="教育背景"/>
    <!-- 项目 -->
    <div class="itemWrapper" v-for="(item,index) in eduData" :key="index">
      <div>
        <svg class="icon" aria-hidden="true">
          <use xlink:href="#icon-icradioture"></use>
        </svg>
        {{item.date}}
      </div>
      <div>{{item.school}}</div>
      <div>{{item.pro}}</div>
    </div>
  </div>
</template>

<script>
import Title from "../components/title/title"
import {eduData} from "../mock/edu"
export default {
  data () {
    return {
      eduData:eduData
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
.eduWrapper{
  margin-top: 32px;
  width: 100%;
}
.itemWrapper{
  display: flex;
  justify-content: space-between;
  margin-top: 16px;
}
.itemWrapper div{
  flex: 1;
  text-align: left;
  color: #0072bd;
  font-weight: 600;
}
</style>