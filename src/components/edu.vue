<!--  -->
<template>
  <div class="eduWrapper">
    <Title titleName="教育背景"/>
    <!-- 项目 -->
    <div class="itemWrapper">
      <div>
        <svg class="icon" aria-hidden="true">
          <use xlink:href="#icon-icradioture"></use>
        </svg>
        2019-09 至 2022-03
      </div>
      <div>南开大学</div>
      <div>计算机科学与技术</div>
    </div>

    <div class="itemWrapper">
      <div>
        <svg class="icon" aria-hidden="true">
          <use xlink:href="#icon-icradioture"></use>
        </svg>
        2015-09 至 2017-07
      </div>
      <div>廊坊职业技术学院</div>
      <div>数字媒体</div>
    </div>
    
  </div>
</template>

<script>
import Title from "../components/title/title"
export default {
  data () {
    return {
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