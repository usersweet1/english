<template>
  <div class="card">
    <div class="record">
        <div class="recordwords">
            <p>学习记录</p>
            <p @click="showModal">联系客服</p> 
            <modal v-if="modalVisiable" @close="onModalClose"></modal>
        </div>
    </div>
  </div>
</template>

<script>

import modal from './modal'
export default {
  data () {
    return {
      modalVisiable: false
    }
  },
  components: {
    modal
  },
  methods: {
    onModalClose () {
      this.modalVisiable = false
    },
    showModal () {
      this.modalVisiable = true
    }
  }
}
</script>

<style scoped>
.record{
    width: 320px;
    height: 500px;
    background-color: white;
    margin: -10px auto;
    border-radius: 2%;
    border:1px solid white;
}
.recordwords{
    margin:10px 20px;
}
p{
    color:#696969;
    display: block;
    margin: 20px 0;
}

</style>
