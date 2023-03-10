<template>
  <v-main class="bg-grey-lighten-3">
    <v-container>
      <v-row>
        <v-col cols="12" sm="2">
          <v-sheet rounded="lg" min-height="268"> </v-sheet>
        </v-col>

        <v-col cols="12" sm="7">
          <v-sheet min-height="70vh" rounded="lg" class="padding">
            <OverviewCard />
          </v-sheet>
        </v-col>

        <v-col cols="12" sm="3">
          <AppWeatherCard />
        </v-col>
      </v-row>
    </v-container>
    <AppNews />
  </v-main>
</template>

<script>
import OverviewCard from './OverviewCard.vue'
import AppNews from './AppNews.vue'
import AppWeatherCard from './AppWeatherCard.vue'

export default {
  name: 'AppBody',
  components: {
    OverviewCard,
    AppNews,
    AppWeatherCard
  }
}
</script>

<style>
.padding {
  padding: 2rem;
}
</style>
