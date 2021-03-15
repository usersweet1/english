<template>
  <div class="pnav">
    <div class="content">
      <div class="container one">
        <image src="/static/images/nav.jpg"></image>
        <navigator url="/pages/list/main">英语阅读</navigator>
      </div>
      <div class="container two">
        <image src="/static/images/navtwo.jpg"></image>
        <h1>英语考试</h1>
      </div>
      <div class="container three">
        <image src="/static/images/words.jpg"></image>
        <div url="/pages/words/main" @click="handle">每日记单词</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    handle() {
      wx.switchTab({
        url: "/pages/words/main",
      });
    },
  },
};
</script>

<style scoped>
.pnav {
  position: relative;
}
.content {
  position: absolute;
  top: 240px;
  left: 17px;
}
.container {
  float: left;
}
image {
  width: 74px;
  height: 74px;
  margin: 0 20px;
}
h1 {
  margin: 0 24px;
}
</style>
