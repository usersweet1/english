<template>
  <div class="logs">
    <personal></personal>
    <personalcard></personalcard>
  </div>
</template>

<script>
import personal from '@/components/personal'
import personalcard from '@/components/personalcard'
export default {
  components: {
    personal,
    personalcard
  }
}
</script>

<style>
.logs{
  background-color: #F5F5F5;
}
</style>
