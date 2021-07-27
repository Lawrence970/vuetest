<template>
  <div id="loginForm">
    <span class="nav-group">
      <p> crt </p>
      <h2 class="large-text-h2">Sign In</h2>
    </span>

    <span class="input-group">
      <input type="text" v-model="logInEmail" placeholder="Email" autofocus/>
      <input type="password" v-model="logInPassword" placeholder=" Password"/>
      <button type="button" class="input-button" v-on:click="logInUser">continue</button>
    </span>

  </div>

</template>

<script>
export default {
  name: 'loginForm',

}
</script>

<style scoped>

/* global variables in landing.vue */

.nav-group {
  background-color: #63b5f7;
  display:flex;
  justify-content:space-between;
}

.large-text-h2 {
  font-size: 2.3em;
  color: #1c1c1c;
  text-align: right;
  font-family: sans-serif;

}

.input-group {
  display: flex;
  flex-direction:column;
  align-items: center;

}


</style>