<template>
  <div id="app">
<small-user-profile v-for="(user, i) in users" :key="i" :user="users[i]"></small-user-profile>
  </div>
</template>

<script>
import SmallUserProfile from "@/components/SmallUserProfile.vue"

export default {

  data() {
    return {
      users: [
        {
          name: `David`,
          age: `26`,
          is_premium: true,
          id: `1738`
        },
        {
         name: `Dav`,
          age: `42`,
          is_premium: false,
          id: `175538`
        },
        {
          name: `Dev`,
          age: `52`,
          is_premium: true,
          id: `17538`
        },
      ]
    };
  },

  name: 'App',
  components: {
SmallUserProfile
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
