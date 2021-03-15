<template>
  <div class="learnwords">
    <div class="header">
      <progress percent="20" stroke-width="6" color="#a4e5f3" />
    </div>
    <div class="container">
      <h1>{{ learnwords }}</h1>
      <h2>{{ symbol }}</h2>
    </div>
    <div class="options">
      <div
        class="option"
        :style="{
          'background-color':
            index === checkedIndex
              ? checkedIndex === rightKey
                ? '#90EE90'
                : '#FA8072'
              : 'white',
        }"
        v-for="(item, index) in wordsoptions"
        :key="index"
        @click="checkedOption(index)"
      >
        <h3>{{ optionFlagMapping[index] }}</h3>
        <p>{{ item }}</p>
      </div>
      <!-- <div class="option">
        <h3>C</h3>
        <p>{{ optionC }}</p>
      </div>
      <div class="option">
        <h3>D</h3>
        <p>{{ optionD }}</p>
      </div> -->
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      wait: 10,
      already: 0,
      learnwords: "access",
      symbol: " [ˈækses]",
      checkedIndex: null,
      optionFlagMapping: { 0: "A", 1: "B", 2: "C", 3: "D" },
      wordsoptions: ["n.入口;通道;方法", "n.合并,归并", "n.闪电", "n.处理不足"],
      rightKey: 1,
    };
  },
  methods: {
    checkedOption(index) {
      this.checkedIndex = index;
    },
  },
};
</script>
<style scoped>
.learnwords {
  display: flex;
  flex-direction: column;
}
.header {
  margin: 10px 10px;
}
.header p {
  margin: 10px 10px 20px;
}

.container {
  text-align: center;
  height: 50px;
  width: 100%;
  margin: -50px auto 20px;
}
h1 {
  font-size: 50px;
  font-weight: bolder;
}
.option {
  display: flex;
  margin: 30px auto;
  width: 280px;
  height: 70px;
  box-shadow: 0 0 8px 1px #dcdcdc;
  text-align: center;
  border-radius: 40px;
}
h3 {
  margin: auto 10px auto 20px;
}
.option p {
  margin: auto 10px;
}
</style>