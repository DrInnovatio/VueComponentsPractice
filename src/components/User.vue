<template>
  <button type="button" @click="onClickAge">Update Age</button>
  <p>The {{firstName}} is {{age}} years old.</p>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "User",
  props: ["age", "firstName"],
  methods: {
    onClickAge() {
      this.$emit('age-change')
    }
  }
}
</script>

<style>

</style>