<!--  -->
<template>
  <div>
    <div class="titleWrapper"> 
      <div class="TitleHeader">
      </div>
      <div class="titleContent">{{titleName}}</div>
      <div class="line"></div>

    </div>
    
  </div>
</template>

<script>
export default {
  props:{
    titleName:{
      type:String,
      default(){
        return ""
      }
    }
  },
  data () {
    return {
    };
  },

  components:{},

  computed:{},

  mounted(){},

  methods:{}
}

</script>
<style scoped>
.titleWrapper{
  position: relative;
}
.TitleHeader{
  position: absolute;
  top: 0px;
  left: 0px;
  border-bottom: 28px solid #0072bd;
  border-left: 0px solid transparent;
  border-right: 20px solid transparent;
  height: 0px; 
  width: 150px;
}
.titleContent{
  position: absolute;
  top: 0px;
  left: 30px;
  color: #fff;
  font-size: 18px;
}
.line{
  width: 100%;
  height: 28px;
  border-bottom: 1px solid #0072bd;
}

</style>