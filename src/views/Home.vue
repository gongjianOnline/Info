<!--  -->
<template>
  <div class="wrapper">
    <header>
      <Header/>
      <Info/>
    </header>
    <nav>
      <Edu/>
    </nav>

  </div>
</template>

<script>
import Header from "../components/header.vue";
import Info from "../components/Info";
import Edu from "../components/edu"
export default {
  data () {
    return {
    };
  },

  components:{
    Header,
    Info,
    Edu
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
  height: 100vh;
  padding-left: 34px;
  padding-right: 34px;
}
</style>