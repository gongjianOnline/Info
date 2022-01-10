<!--  -->
<template>
  <div class="InfoWrapper">
    <div class="left">
      <h1>龚 箭</h1>
      <h2>在探索的路上永不止步</h2>
      <!-- 个人信息 -->
      <div class="infoContainer marginTop">
        <div>
          <span class="dot"></span>
          性别:
          <span class="infoValue">男</span>
        </div>
        <div>
          <span class="dot"></span>
          年龄:
          <span class="infoValue">25</span>
        </div>
      </div>
      <div class="infoContainer interval">
        <div>
          <span class="dot"></span>
          学历:
          <span class="infoValue">本科</span>
        </div>
        <div>
          <span class="dot"></span>
          工作年限:
          <span class="infoValue">4年</span>
        </div>
      </div>
      <div class="infoContainer interval">
        <div>
          <span class="dot"></span>
          联系电话:
          <span class="infoValue">暂不开放</span>
        </div>
        <div>
          <span class="dot"></span>
          电子邮箱:
          <span class="infoValue">gjwebTop@163.com</span>
        </div>
      </div>
      <div class="infoContainer interval">
        <div>
          <span class="dot"></span>
          技术博客:
          <span class="infoValue">
            <a href="http://www.gjweb.top" target="_blank">点此进入</a>
          </span>
        </div>
        <div>
          <span class="dot"></span>
          gitHub:
          <span class="infoValue">
            <a href="https://github.com/gongjianOnline" target="_blank">点此进入</a>
          </span>
        </div>
      </div>
    </div>
    <div class="right">
      <img src="" alt="" class="imgLogo">
    </div>
  </div>
</template>

<script>
export default {
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
.InfoWrapper{
  display: flex;
  justify-content: space-between;
  width: 100%;
  min-height: 200px;
  margin-top: 10px;
}
.left{
  width: 70%;
}
.right{
  width: 20%;
}
h1{
  text-align: left;
  margin: 0;
  font-size: 30px;
  font-weight: 500;
}
h2{
  text-align: left;
  margin: 0;
  margin-top: 14px;
  font-size: 16px;
  font-weight: 400;
  color: rgb(92, 91, 91);
}
/* 个人信息 */
.marginTop{
  margin-top: 36px;
}
.interval{
  margin-top: 12px;
}
.infoContainer{
  border-bottom: 1px solid #f1f1f1;
  display: flex;
  padding-bottom: 12px;
}
.infoContainer>div{
  flex: 1;
  text-align: left;
}
.dot{
  display: inline-block;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: #0072bd;
  margin-right: 8px;
}
.infoValue{
  display: inline-block;
  margin-left: 12px;
}
.imgLogo{
  border: 3px solid #e5e5e5;
  width: 100%;
  height: 180px;
  margin-top: 6px;
}
</style>