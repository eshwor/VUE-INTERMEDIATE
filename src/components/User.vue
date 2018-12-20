<template>
  <div class="user-div">
    <h1> This is the User Page</h1>
    <button type="button" name="button" @click="changeName">Change Name</button>
    <UserDetail :myName="name" @nameWasReset="name = $event"></UserDetail>
  </div>
</template>

<script>
import UserDetail from './UserDetail.vue'
export default {
  data () {
    return {
      name: 'Vue'
    }
  },
  methods: {
    changeName () {
      this.name = 'Wonderful VueJS'
    }
  },
  components: {
    UserDetail
  }
}
</script>
