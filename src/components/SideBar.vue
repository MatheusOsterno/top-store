<template>
    <v-app id="inspire">
      <v-navigation-drawer
        v-model="drawer"
        app
        class="pt-4"
        color="grey lighten-3"
        expand-on-hover
        mini-variant
      >
      <v-list-item class="px-2">
        <v-list-item-avatar>
          <v-img src="Matheus-Osterno.jpg"></v-img>
        </v-list-item-avatar>

        <v-list-item-title>John Leider</v-list-item-title>

      </v-list-item>

      <v-divider></v-divider>

      <v-list dense>
        <v-list-item
          v-for="item in items"
          :key="item.title"
          link
        >
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
  
      <v-main>
       
      </v-main>
    </v-app>
  </template>

<script>
export default {
    data () {
      return {
        drawer: true,
        items: [
          { title: 'Home', icon: 'mdi-home-city' },
          { title: 'My Account', icon: 'mdi-account' },
          { title: 'Users', icon: 'mdi-account-group-outline' },
        ],
        mini: true,
      }
    },
}
</script>

<style>
* {
    border-width: 0px;
}
</style>