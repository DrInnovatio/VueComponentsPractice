<template>
  <h3>hey</h3>
  <button type="button" @click="age++">Update Age</button>
  <greeting :age="age"></greeting>
  <user :age="age" @age-change="updateAge" :firstName="firstName"></user>
</template>

<script>

import Greeting from "./components/Greeting.vue"
import User from "./components/User.vue"

  export default {
    name: "App",
    components: {
      Greeting,
      User, 
    },
    data(){
      return {
        age: 20,
        firstName: "James"
      }
    },
    methods: {
      updateAge(num){
        this.age += num;
      }
    }

  }
</script>

<style> 

</style>
