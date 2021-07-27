<template>
  <div id="adminPage">
    <h1 class="large-text-h1">Welcome {{ currentUser.company.company_name }}</h1>
    <button class="logout-button">logout</button>
    <button class="input-button" v-on:click="goToDisplayAllDrivers">All Drivers</button>
    <button class="input-button" v-on:click="type_role=`user`">Add New Driver</button>



  </div>
</template>

<script>

export default {
  name: 'adminPage',

}
</script>

<style>

</style>