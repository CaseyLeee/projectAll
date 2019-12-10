<template>
  <div id="app">
    <!--顶部header-->
    <mt-header fixed title="UPUP">
      <router-link to="/" slot="left">
        <mt-button icon="back">返回</mt-button>
      </router-link>
    </mt-header>

    <!--路由区MINTUI-->
    <!-- <mt-tab-container v-model="active">
      <mt-tab-container-item id="tab1">
        <h1 v-for="(item,i) in [1,2,3]" :key=i>{{item}}</h1>
      </mt-tab-container-item>
      <mt-tab-container-item id="tab2">
        <h1 v-for="(item,i) in [4,5,6]" :key=i>{{item}}</h1>
      </mt-tab-container-item>
      <mt-tab-container-item id="tab3">
        <h1 v-for="(item,i) in [7,8,9]" :key=i>{{item}}</h1>
      </mt-tab-container-item>
      <mt-tab-container-item id="tab4">
        <h1 v-for="(item,i) in [10,11,12]" :key=i>{{item}}</h1>
      </mt-tab-container-item>
    </mt-tab-container> -->
    <!--顶部tab区域-->
    <!-- <mt-tabbar v-model="active" fixed>
      <mt-tab-item id="tab1">
        <img slot="icon" src="./image/chicken.jpg">
        外卖
      </mt-tab-item>
      <mt-tab-item id="tab2">
        <img slot="icon" src="./image/chicken.jpg">
        订单
      </mt-tab-item>
      <mt-tab-item id="tab3">
        <img slot="icon" src="./image/chicken.jpg">
        发现
      </mt-tab-item>
      <mt-tab-item id="tab4">
        <img slot="icon" src="./image/chicken.jpg">
        我的
      </mt-tab-item>
    </mt-tabbar> -->
    <nav class="mui-bar mui-bar-tab">
      <a class="mui-tab-item mui-active" href="#tabbar">
        <span class="mui-icon mui-icon-home"></span>
        <span class="mui-tab-label">首页</span>
      </a>
      <a class="mui-tab-item" href="#tabbar-with-chat">
        <span class="mui-icon mui-icon-email"><span class="mui-badge">9</span></span>
        <span class="mui-tab-label">消息</span>
      </a>
      <a class="mui-tab-item" href="#tabbar-with-contact">
        <span class="mui-icon mui-icon-contact"></span>
        <span class="mui-tab-label">通讯录</span>
      </a>
      <a class="mui-tab-item" href="#tabbar-with-map">
        <span class="mui-icon mui-icon-gear"></span>
        <span class="mui-tab-label">设置</span>
      </a>
    </nav>


  </div>
</template>

<script>
  export default {
    name: 'App',
    data() {
      return {
        active: 'tab1'
      };
    }
  }

</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }

</style>
