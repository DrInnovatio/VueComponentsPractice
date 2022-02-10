<template>
  <p>The {{firstName}} is {{age}} years old.</p>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "User",
  props: ["age", "firstName"]
}
</script>

<style>

</style>