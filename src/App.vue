<!-- This is the file where you can merge all the component together -->
<template>
  <div id="main-app">
    <NewComponent></NewComponent>
  </div>
</template>

<script>
import NewComponent from './components/TestComponent'
export default {
  name: 'app',
  components: {
    'NewComponent': NewComponent
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
