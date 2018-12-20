<!-- This is the file where you can merge all the component together -->
<template>
  <div id="main-app">
    <User></User>
  </div>
</template>

<script>
import User from './components/User'
export default {
  name: 'app',
  components: {
    User
  }
}
</script>

<style scoped>
  h1 {
     color: blue;
     text-align: center;
 }
 #main-app {
   text-align: center;
 }
</style>
