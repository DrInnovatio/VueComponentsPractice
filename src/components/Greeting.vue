/* eslint-disable vue/multi-word-component-names */
<template>
  <p>{{msg}}</p>
</template>

<script>

  export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Greeting",
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