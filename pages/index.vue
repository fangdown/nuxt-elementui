<template>
  <div class="wrap">
    <header>头部</header>
    <div class="container" flex="main:left">
      <div class="slide">侧边</div>
      <div class="main" flex-box=1>内容</div>
    </div>
  </div>
</template>

<script>
import Logo from '~components/Logo.vue'

export default {
  components: {
    Logo
  },
  data () {
    return {
      name: ''
    }
  }
}
</script>

<style>
  header {
    height:80px;
    border-bottom: 1px solid #ddd;
  }
  .wrap {
    position: absolute;
    top: 0;
    bottom: 0;
    width: 100%;
  }
  .head {
    height: 80px;
    border-bottom: 1px solid #ddd;
  }
  .container {
    position: absolute;
    top: 80px;
    bottom: 0;
    overflow: hidden;
  }
  .slide {
    width:200px;
    border-right: 1px solid #ddd;
  }
</style>
