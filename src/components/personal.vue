<template>
  <div class="personal">
    <div class="face">
      <img src="/static/images/face.jpg" alt="" />
    </div>
    <div class="name">
      <p>小甜心</p>
      <p>ID:520520</p>
    </div>
  </div>
</template>

<script>
</script>

<style>
.personal {
  width: 100%;
  height: 120px;
  background-color: #a4e5f3;
  border: 1px solid #a4e5f3;
  display: flex;
  flex-direction: row;
}
.face {
  width: 70px;
  height: 70px;
  border-radius: 50%;
  border: 2px solid white;
  overflow: hidden;
  margin: 20px 20px;
}
.face img {
  width: 70px;
  height: 70px;
}
.name {
  width: 100px;
  height: 100px;
  margin: 20px 20px;
}
p {
  color: white;
  display: block;
  margin: 10px 0;
}
</style>
