<template>
  <v-app>
    <v-navigation-drawer v-model="drawer" app>
      <v-list-item link>
        <nuxt-link to="/">Home page</nuxt-link>
      </v-list-item>
      <v-list-item link>
        <nuxt-link to="/fun">Fun page</nuxt-link>
      </v-list-item>
      <v-list-item link>
        <nuxt-link to="/more-fun">More fun page</nuxt-link>
      </v-list-item>
    </v-navigation-drawer>
    <v-app-bar app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title>Application</v-toolbar-title>
    </v-app-bar>
    <v-main>
      <nuxt />
    </v-main>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data() {
    return {
      drawer: null
    }
  }
})
</script>
