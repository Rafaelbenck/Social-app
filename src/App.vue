<template>
  <v-app id="inspire">
    <AppHeader />
    <AppBody />
  </v-app>
</template>

<script>
import AppBody from './components/AppBody.vue'
import AppHeader from './components/AppHeader.vue'

export default {
  name: 'App',

  components: {
    AppHeader,
    AppBody
  },

  data: () => ({})
}
</script>
