<!--  -->
<template>
  <div class="wrapper">
    <header>
      <Header/>
      <Info/>
    </header>
    <nav><Edu/></nav>
    <nav><Skill/></nav>

  </div>
</template>

<script>
import Header from "../components/header.vue";
import Info from "../components/Info";
import Edu from "../components/edu";
import Skill from "../components/skill"
export default {
  data () {
    return {
    };
  },

  components:{
    Header,
    Info,
    Edu,
    Skill
  },

  computed:{},

  mounted(){},

  methods:{}
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