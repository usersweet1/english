<template>
  <div class="card">
    <image src="/static/images/sen.jpg"></image>
    <div class="cardm">
      <p>
        Life is just like that sometimes, we’re hoping for a unicorn and we get
        a goat.
      </p>
      <p>有时候人生就是如此，我们期待的是独角兽，得到的却是山羊。</p>
    </div>
    <button id="btn" :disabled="clockFlag" @click="clockOff">打卡</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      clockFlag: false,
    };
  },
  methods: {
    clockOff() {
      this.clockFlag = !this.clockFlag;
    },
  },
};
</script>

<style scoped>
.card {
  position: relative;
}
image {
  width: 100%;
  height: 210px;
}
.cardm {
  width: 350px;
  height: 210px;
  background-color: white;
  text-align: center;
  margin: -40px 12px 0;
  border: 1px solid #bbbbbe;
  z-index: 1;
  position: absolute;
  border-radius: 10px;
}
.card p {
  margin: 24px 18px;
  font-size: 18px;
}
button {
  width: 125px;
  height: 57px;
  position: absolute;
  top: 360px;
  left: 200px;
  z-index: 2;
  text-align: center;
  background-color: #a4e5f3;
  line-height: 57px;
}
.zhihui {
  background-color: #555555;
}
</style>
