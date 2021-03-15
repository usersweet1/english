<template>
  <div class="words">
    <div class="header">
      <img src="/static/images/orders.png" alt="" />
      <div class="header_content">
        <p>已学单词</p>
        <span>{{ wordsNum }}</span>
      </div>
      <div class="header_contentt">
        <p>打卡天数</p>
        <span>{{ dayNum }}</span>
      </div>
      <div class="cardm">
        <div class="re">
          <h1>剩余单词:{{ remainingWords }}</h1>
          <button id="studybtn">学习计划</button>
        </div>
        <div class="container">
          <div class="today">
            <span>{{ today }}</span>
            <p>今日剩余</p>
          </div>
          <div class="book">
            <span>{{ book }}</span>
            <p>本书已学</p>
          </div>
          <div class="day">
            <span>{{ day }}</span>
            <p>剩余天数</p>
          </div>
        </div>

        <button id="btn" @click="clockOff">开始学习</button>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      wordsNum: 0,
      dayNum: 0,
      remainingWords: 0,
      today: 0,
      book: 0,
      day: 0,
    };
  },
  methods: {
    clockOff() {
      wx.navigateTo({
        url: "/pages/learnwords/main",
      });
    },
  },
};
</script>
<style scoped>
.header {
  width: 100%;
  height: 300px;
  background-color: #a4e5f3;
  position: relative;
}
img {
  width: 30px;
  height: 30px;
  position: absolute;
  top: 10%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.header_content {
  position: absolute;
  top: 100px;
  left: 80px;
  text-align: center;
}
span {
  font-size: 30px;
}

.header_contentt {
  position: absolute;
  top: 100px;
  left: 230px;
  text-align: center;
}
.cardm {
  width: 350px;
  height: 380px;
  background-color: white;
  margin: 20px 12px 0;
  border: 1px solid #bbbbbe;
  z-index: 1;
  position: absolute;
  top: 200px;
  border-radius: 10px;
}
.re {
  width: 300px;
  height: 40px;
  margin: 20px auto;
  border-bottom: 1px solid #bbbbbe;
}
.re h1 {
  margin-bottom: 10px;
  font-size: 15px;
  display: inline-block;
}
#studybtn {
  width: 80px;
  height: 25px;
  font-size: 12px;
  display: inline-block;
  float: right;
  text-align: center;
  line-height: 25px;
}
.container {
  text-align: center;
}
.today {
  position: absolute;
  left: 20px;
  top: 120px;
}
.book {
  position: absolute;
  left: 150px;
  top: 120px;
}
.day {
  position: absolute;
  left: 270px;
  top: 120px;
}
#btn {
  width: 140px;
  height: 40px;
  position: absolute;
  top: 280px;
  left: 110px;
  z-index: 2;
  text-align: center;
  background-color: #a4e5f3;
  line-height: 40px;
  font-size: 15px;
}
</style>