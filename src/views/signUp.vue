<template>
    <div id="signUpPage">

    <h2 class="large-text-h2">Create Your Account</h2>


    <hr>

    <span class="justify-between">
        <input type="text"      class="input-field"  v-model="new_company_email" placeholder="Email" autofocus/>
        <input type="password"  class="input-field"  v-model="new_company_name" placeholder="Company"/>
        <input type="password"  class="input-field"  v-model="new_company_password" placeholder="password"/>
        <input type="password"  class="input-field"  v-model="new_company_confirm_password" placeholder="confirm password"/>
        <button type="button"   class="input-button" v-on:click="addNewUser">continue</button>
        <p class="para-text">Already Have an Account?</p>
        <button type="button"   class="input-button" v-on:click="type_role=`company`" >Sign In!</button>
    </span>

        
        
    </div>
</template>

<script>
export default {
    name: 'signUpPage',

}
</script>

<style>
/* styles are global here */
body {
    --color-primary: #008cff; 
    --color-secondary: #1c1c1c;
    --color-error: #cc3333;
    --color-success: #4bb544;


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

.large-text-h2 {
    font-size: 2em;
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
    padding-left: 6px;
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

.logout-button {
    background-color: var(--color-error);
}




</style>