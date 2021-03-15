<template>
  <div class="list">
    <div class="content">
      <div class="EnglishWords">
        <p>
           China will become the largest foreign capital inflowcountry in the world in 2020
        </p>
      </div>
      <div class="describe">
        <div class="img">
          <img src="/static/images/china.jpg" alt="">
        </div>
        <div class="title">
          <h1>
            2020中国成为全球最大外资流入国
          </h1>
        </div>
      </div>
    </div>
    <div class="content">
      <div class="EnglishWords">
        <p>
           Beijing releases new rules for Spring Festival
        </p>
      </div>
      <div class="describe">
        <div class="img">
          <img src="/static/images/beijing.jpg" alt="">
        </div>
        <div class="title">
          <h1>
            北京发布春节进返京新规
          </h1>
        </div>
      </div>
    </div>
    <div class="content">
      <div class="EnglishWords">
        <p>
           Thousands of Americans cross state vaccinations
        </p>
      </div>
      <div class="describe">
        <div class="img">
          <img src="/static/images/USA.jpg" alt="">
        </div>
        <div class="title">
          <h1>
            成千上万的美国人跨州接种疫苗
          </h1>
        </div>
      </div>
    </div>
  </div>
</template>
<script>

</script>

<style scoped>
.content{
  width: 350px;
  height: 230px;
  border: 1px solid #BBBBBB;
  margin: 20px auto 40px;
}
.EnglishWords{
  height: 60px;
  width: 100%;
  border-bottom: 1px solid #BBBBBB;
}
.EnglishWords p{
  display: block;
  margin: 30px 10px;
  width: 100%;
  height: 60px;
}
.img{
  width: 184px;
  height: 130px;
  position: relative;
}
img{
  width: 170px;
  height: 100px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
}
.title{
  width: 150px;
  height: 120px;
  position: relative;
  left: 200px;
  top: -100px;
}
.title h1{
  width: 150px;
  height: 94px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
}
</style>