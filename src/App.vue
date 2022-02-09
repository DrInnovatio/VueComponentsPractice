<template>
  <h3>hey</h3>
  <greeting></greeting>
  <user></user>
</template>

<script>

import Greeting from "./components/Greeting.vue"
import User from "./components/User.vue"

  export default {
    name: "App",
    components: {
      Greeting,
      User,
    }
  }
</script>

<style> 

</style>
