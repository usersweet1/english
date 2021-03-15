<template>
<div class="modalMask" @click="onModalClose">
  <div class="modal" @click.stop>
    <div class="content">
      <img src="/static/images/erweima.png" alt="">
      <p>请扫描二维码联系客服</p>
    </div>
  </div>
  </div>
</template>

<script>
export default {
  props: {
    visiable: {
      type: Boolean,
      default: false
    }
  },
  methods: {
    onModalClose () {
      this.$emit('close')
    }
  }
}
</script>

<style scoped>
.modalMask{
   width: 100%;
   height: 100%;
   position: fixed;
   top: 0;
   left: 0;
   background-color: rgba(0,0,0,.4);
 }
.modal{
  border-radius: 2%;
  background-color: white;
  width: 300px;
  height: 290px;
  border:1px solid white;
  margin:140px auto;
  position: relative;
}
.content{
  width: 200px;
  height: 200px;
  position: absolute;
  top:50%;
  left:50%;
  transform:translate(-50%,-50%);
}
img{
  width: 180px;
  height: 180px;
  display: block;
  margin: auto;
}
p{
  color:#000000;
  display: block;
  text-align: center;
}
</style>
