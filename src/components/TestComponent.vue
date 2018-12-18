<!-- This is the test component -->
<template>
  <div class="test-component">
    <button type="button" name="button" @click="changeStatus">Change Server Status</button>
    <button type="button" @click="YesNo = !YesNo "> YesNo </button>
    <p> {{YesNo}} </p>
    <h1> Server Status:  {{ ServerStatus }} </h1>
    <hr>
  </div>
</template>

<script>
export default {
  data () {
    return {
      YesNo: false,
      ServerStatus: 'poor'
    }
  },
  methods: {
    changeStatus () {
      this.ServerStatus = 'Normal'
    }
  }
}
</script>

<style scoped>
  button {
    padding: 0.5rem 1rem;
    background-color: blue;
    color: white;
    cursor: pointer;
  }
</style>
