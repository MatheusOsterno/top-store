<template>
  <v-app :style="{ background: $vuetify.theme.themes.dark.background}">
    <SideBar />
    <v-container fluid >

    </v-container>
  </v-app>
</template>

<script>
  import HelloWorld from '../components/HelloWorld'
  import SideBar from '../components/SideBar.vue'

  export default {
    name: 'Home',

    components: {
    SideBar
},
  }
</script>

// <projectRoot>/src/views/.eslintrc.js
  module.exports = {
    rules: {
      'vue/multi-word-component-names': 0,
    },
  }
