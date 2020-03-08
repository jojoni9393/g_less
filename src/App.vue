<template>
  <div id="app">
    <div class="test">g_less</div>
  </div>
</template>


<style lang="less">
@import './assets/css/variables.less';
.test {
  height: 100px;
  width: 100px;
  background-color: @theme_color_btn_a;
}
</style>
