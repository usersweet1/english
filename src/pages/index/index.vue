<template>
  <div class="main">
      <card></card>
      <calendar></calendar>
      <pnav></pnav>
  </div>
</template>

<script>
import card from '@/components/card'
import calendar from '@/components/calendar'
import pnav from '@/components/pnav'
export default {
  components: {
    card,
    calendar,
    pnav
  }}
</script>

<style scoped>

</style>
