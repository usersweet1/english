<template>
  <div class="calendar">
      <div class="body">
           <h1>本周打卡</h1>
           <div class="circle">
               <div class="circlee one">一</div>
               <div class="circlee two">二</div>
               <div class="circlee three">三</div>
               <div class="circlee four">四</div>
               <div class="circlee five">五</div>
               <div class="circlee six">六</div>
               <div class="circlee seven">七</div>
           </div>
      </div>

  </div>
</template>

<script>


</script>

<style scoped>
.calendar{
    position: relative;
}
.body{
    position: absolute;
    top:220px;
    left: 17px;
}
h1{
    font-size: 20px;
}
.circle{
    margin: 15px 0;
}
.circlee{
    background-color: white;
    border-radius: 50px;
    height: 40px;
    width:40px;
    border:1px solid #BBBBBE;
    text-align: center;
    line-height: 40px;
    float: left;
    margin-right:10px;
}

</style>
