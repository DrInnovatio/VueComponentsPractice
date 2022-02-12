<template>
  <button type="button" @click="onClickAge">Update Age</button>
  <p>The {{firstName}} is {{age}} years old.</p>
  <p>{{ageDoubled}}</p>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "User",
  props: {
    age:{
      type: Number,
      //required: true,
      //default: 20
      validator(value){
        this.onClickAge();
        return value < 130
      }
    },
    firstName: {
      type: String,
      //required: true
      
    }
  },
  emits: ['age-change'], 
  computed: {
    ageDoubled(){
      return this.age * 2;
    }
  },
  methods: {
    onClickAge() {
      this.$emit('age-change', 3)
    }
  }
}
</script>

<style>

</style>