<template>
  <main>
    <h1>Hello world!</h1>
    Now: {{ date }}
    <nav>
      <ul>
        <li>
          <nuxt-link to="/fun">Fun page</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/more-fun">More fun page</nuxt-link>
        </li>
      </ul>
    </nav>
  </main>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data() {
    const date = new Date().toString()
    return {
      date
    }
  }
})
</script>
