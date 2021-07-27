<template>
  <div id="driverPage">
    <h1 class="large-text-h1">Welcome {{ currentUser.first_name }}</h1>
    <button class="logout-button">logout</button>
    <button class="input-button" v-on:click="changePageDisplay('myRoutes'), getRoutes()">My Routes</button>
    <button class="input-button" v-on:click="changePageDisplay('newRoute')">New Route</button>




  </div>
</template>

<script>

export default {
  name: 'driverPage',

}
</script>

<style>

</style>