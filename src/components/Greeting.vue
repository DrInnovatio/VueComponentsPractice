/* eslint-disable vue/multi-word-component-names */
<template>
  <p v-if="age > 25">{{msg}}</p>
  <p v-else>You must be 25 years old or older to view this message.</p>
</template>

<script>

  export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Greeting",
    props: ['age'],
    data(){
      return {
        msg: "Kiil Putin."
      };
    }
  }

</script>
 
<style scoped lang="scss">
  $color: rgb(0, 255, 102);

  p {
    color: $color;
    text-align: center;
    background-color: blueviolet;
  }
</style>