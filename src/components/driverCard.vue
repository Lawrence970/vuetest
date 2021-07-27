<template>
  <div id="driverCard">
      <ul>
          <li v-on:click="goToDriver(driver)">
              <span> {{ driver.first_name }} {{ driver.last_name }} </span>
              <span class="driver-id"> {{ "_" + driver._id.slice(driver._id.length - 5) }} </span>
              <p class="para-text">click to see routes</p>
          </li>
      </ul>
  </div>
</template>

<script>
export default {
    name: 'driverCard'
}
</script>

<style>

</style>