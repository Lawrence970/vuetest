<template>
  <div id="landingPage">
    
    <h1 class="large-text-h1">Track The Truck</h1>
    <p class="para-text">Keeping Track of Miles for Miles and Miles</p>

    <hr>

    <span class="justify-between">
        <button type="button"  class="input-button">Sign In</button>
        <button type="button" v-on:click="type_role=`company`" class="input-button">Sign Up</button>
    </span>
    
      
      
  </div>
  
</template>


<script>
export default {
    name: 'landingPage',

}
</script>

<!-- * begining of styles for this component -->
<!-- * without using the scoped option on the style tag, all styles are now global across components -->
<style >

#landingPage {
    padding:0;
    margin-left:150px;
    margin-right:150px;
}

.large-text-h1 {
    font-size: 2.3em;
    color: #1c1c1c;
    text-align: center;
    font-family: sans-serif;
}

.para-text {
    text-align: center;
}

.justify-between {
    display: flex;
    justify-content: space-between;

}

hr {
    width: 35%;
    align-content: center;
}

.input-button {
    width: 200px;
    height: 40px;
    margin: 0;
    margin: 20px;
    border-radius: 50px;
    border: none;
    outline: none;
    color: white;
    padding: 5px;
    background-color: #008cff;
    box-shadow: 4px 6px 8px 2px rgb(0 0 0 / 10%);
    font-size: 1.4em;
}


/* media query for iPhone 5, temporary */
@media screen, (min-width: 320px) and (max-width: 767) {

    #landingPage {
    padding:0;
    margin:0;
    }

    .justify-between {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    }

}
/* <<<<< end media query */
</style>