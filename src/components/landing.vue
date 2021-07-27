<template>
  <div id="landingPage">
    
    <h1 class="large-text-h1">Track The Truck</h1>
    <p class="para-text">Keeping Track of Miles for Miles and Miles</p>

    <hr>

    <span class="justify-between">
        <input type="text"      class="input-field"  v-model="logInEmail" placeholder="Email" autofocus/>
        <input type="password"  class="input-field"  v-model="logInPassword" placeholder=" Password"/>
        <button type="button"   class="input-button" v-on:click="logInUser">continue</button>
        <p class="para-text">Need An Account?</p>
        <button type="button"   class="input-button" v-on:click="type_role=`company`" >Sign Up!</button>
    </span>
    
      
      
  </div>
  
</template>


<script>

export default {
    name: 'landingPage',

}
</script>

<style >

/* ! ALL STYLES IN THIS COMPONENT ARE GLOBAL UNLESS SCOPED!!! */

body {
    --color-primary: #008cff; 
    --color-secondary: #1c1c1c;


    margin:0;
    padding:0;
}

hr {
    width: 100%;
    align-content: center;
}

#landingPage {
    padding:0;
    margin-left:150px;
    margin-right:150px;
    font-family: sans-serif;
}

.large-text-h1 {
    font-size: 2.3em;
    color: var(--color-secondary);
    text-align: center;

}

.para-text {
    text-align: center;
    font-size: 110%;
}

.justify-between {
    display: flex;
    justify-content: space-between;

}

.input-field {
    width: 300px;
    height: 40px;
    margin: 20px;
    border-radius: 50px;
    border: none;
    outline: none;
    color: var(--color-secondary);
    padding: 5px;
    background-color: white;
    box-shadow: 2px 0px 2px 2px rgb(0 0 0 / 10%);
    font-size: 1.4em;
}

.input-button {
    width: 200px;
    height: 40px;
    margin: 20px;
    border-radius: 50px;
    border: none;
    outline: none;
    color: white;
    padding: 5px;
    background-color: var(--color-primary);
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