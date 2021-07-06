<template>
  <q-page class="flex flex-center">
    
  </q-page>
</template>

<script>
  import api from '../services/api.js'

  export default {
    name: "PageIndex",

    beforeMount() {
    // Make a request for a user with a given ID
    api.get('pokemon/157/')
      .then( (response) => {
        // handle success
        console.log(response);
      })
      .catch( (error) =>{
        // handle error
        console.log(error);
      })
      .then( () =>{
        // always executed
      });


  }
}  

import { defineComponent } from 'vue';







</script>
