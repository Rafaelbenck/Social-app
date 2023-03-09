<template>
  <div>
    <v-app-bar class="px-3" color="white" flat density="compact">
      <v-avatar color="grey-darken-1" size="32"></v-avatar>

      <v-spacer></v-spacer>

      <v-tabs centered color="grey-darken-2">
        <v-tab v-for="link in links" :key="link">
          {{ link }}
        </v-tab>
      </v-tabs>
      <v-spacer></v-spacer>
    </v-app-bar>
  </div>
</template>

<script>
export default {
  name: 'AppHeader',
  data: () => ({
    links: ['Dashboard', 'Messages', 'Profile', 'Updates']
  })
}
</script>
