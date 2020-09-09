<template>
  <v-container>
    <h1>Hello world!</h1>
    Now: {{ date }}
  </v-container>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data() {
    const date = new Date().toString()
    return {
      date,
    }
  }
})
</script>
