<template>
  <div id="allDriversPage">
      <p>Back</p>
      <h2 class="large-text-h2">All Drivers</h2>
      <driverCard/>
  </div>
</template>

<script>
import driverCard from './driverCard.vue'

export default {
    name: 'allDriversPage',
    components: { driverCard }
}
</script>

<style>

</style>