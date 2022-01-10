<!--  -->
<template>
  <div class="wrapper" ref="exportPdf">
    <header>
      <Header/>
      <Info/>
    </header>
    <nav><Edu/></nav>
    <nav><Skill/></nav>
    <nav><Work/></nav>
    <nav><Project/></nav>

  </div>
</template>

<script>
import Header from "../components/header.vue";
import Info from "../components/Info";
import Edu from "../components/edu";
import Skill from "../components/skill";
import Work from "../components/work";
import Project from "../components/project"
export default {
  data () {
    return {
    };
  },

  components:{
    Header,
    Info,
    Edu,
    Skill,
    Work,
    Project
  },

  computed:{},

  mounted(){},

  methods:{
    xxx(){
      this.$PDFSave(this.$refs.exportPdf, "我的文件");
    }
  }
}

</script>
<style scoped>
.wrapper{
  width:794px;
  margin: 10px auto;
  background: #fff;
  padding-left: 34px;
  padding-right: 34px;
}
</style>