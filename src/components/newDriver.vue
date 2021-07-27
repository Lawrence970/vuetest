<template>
  <div id="newDriver">
    <span class="menu">
        <button class="logout-button" v-on:click="changePageDisplay('adminPage')">cancel</button>
    </span>

    <h2 class="large-text-h2">New Driver</h2>
    <span class="justify-between">
        <input type="text"      class="input-field"  v-model="email" placeholder="email" autofocus/>
        <input type="password"  class="input-field"  v-model="first_name" placeholder="first name"/>
        <input type="password"  class="input-field"  v-model="last_name" placeholder="last name"/>
        <input type="password"  class="input-field"  v-model="password" placeholder="password"/>
        <input type="password"  class="input-field"  v-model="confirm_password" placeholder="confirm password"/>
        <button type="button"   class="input-button" v-on:click="addNewUser">continue</button>
    </span>

  </div>
</template>

<script>
export default {
    name: 'newDriver',
}
</script>

<style>

</style>