<template>
  <v-main class="bg-grey-lighten-3">
    <v-container>
      <v-row>
        <v-col cols="12" sm="2">
          <v-sheet rounded="lg" min-height="268"> </v-sheet>
        </v-col>

        <v-col cols="12" sm="8">
          <v-sheet min-height="70vh" rounded="lg" class="padding">
            <OverviewCard />
            <OverviewCard />
            <OverviewCard />
          </v-sheet>
        </v-col>

        <v-col cols="12" sm="2">
          <v-sheet rounded="lg" min-height="268"> </v-sheet>
        </v-col>
      </v-row>
    </v-container>
  </v-main>
</template>

<script>
import OverviewCard from './OverviewCard.vue'

export default {
  name: 'AppBody',
  components: {
    OverviewCard
  }
}
</script>

<style>
.padding {
  padding: 2rem;
}
</style>
