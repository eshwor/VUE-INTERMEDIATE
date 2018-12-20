<template>
  <div class="user-detail">
    <h1>The user name is : {{ myName }}</h1>
    <button type="button" name="button" @click="resetName">Reset Name</button>
    <!-- <h1>The user name is : {{ switchName() }}</h1> -->
  </div>
</template>

<script>
export default {
  // props: ['myName'],
  props: {
    myName: {
      type: String,
      default: 'Default Value'
    }
  },
  methods: {
    resetName () {
      this.myName = 'Angular'
      this.$emit('nameWasReset', this.myName)
    }
    // switchName () {
    //   return this.myName.split('').reverse().join('')
    // }
  }
}
</script>

<style scoped>
.user-detail {
  background-color: green;
  color: white;
  padding: 1rem;
  margin-top: 1rem;
}
</style>
