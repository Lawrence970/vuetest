<template>
  <div class="landingPage">
      <h1>Track The Truck</h1>
      <p>keeping track of miles for you</p>
      <button type="button" v-on:click="changePageDisplay('signIn') " class="input-button">Sign In</button>
      <button type="button" v-on:click="changePageDisplay('signUp'), type_role=`company`" class="input-button">Sign Up</button>
  </div>
</template>


<script>
export default {
    name: 'landing',

}
</script>

<style>

.app-name-h1 {
    font-size: 1.4em;
    color:cadetblue;
    text-align: center;
}

.input-button {
    width: 200px;
    height: 80px;
    margin: 0;
    padding: 5px;
    background-color: rgb(104, 104, 206);
    box-shadow: 12px 12px 2px 1px rgba(0, 0, 255, .2);
}

</style>