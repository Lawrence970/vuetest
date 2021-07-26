<!-- ??? This file is where everything gets compiled, it then goes to index.html to be injected -->
<template>
  <loginForm/>
 
</template>

<script>

// * this is where all of the components you want are IMPORTED
import loginForm from './components/loginForm.vue'


// * everything in the application is 'stored' here in the export default option/object
export default {
  name: 'App',
  // * this is where all of the components are EXPORTED; injected into index.html
  components: {
    loginForm,
    
  }
}
</script>

<style>
/* ? this styling for the div container with id=app */

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  margin:0 auto;
  padding:0 auto;
}
</style>
