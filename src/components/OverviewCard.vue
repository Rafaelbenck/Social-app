<template>
  <v-card class="mx-auto" max-width="344" variant="outlined" style="margin: 2rem 0">
    <v-card-item>
      <div>
        <div class="text-overline mb-1">OVERLINE</div>
        <div class="text-h6 mb-1">Headline</div>
        <div class="text-caption">Greyhound divisely hello coldly fonwderfully</div>
      </div>
    </v-card-item>

    <v-card-actions>
      <v-btn variant="outlined"> Button </v-btn>
    </v-card-actions>

    <br />

    <v-row justify="space-around">
      <v-col cols="auto">
        <v-sheet>
          <v-chip-group multiple selected-class="text-primary">
            <v-chip v-for="tag in tags" :key="tag">
              {{ tag }}
            </v-chip>
          </v-chip-group>
        </v-sheet>
      </v-col>
    </v-row>
  </v-card>
</template>

<script>
export default {
  name: 'OverviewCard',
  data: () => ({
    tags: ['Best seller', 'Most view', 'Other text']
  })
}
</script>

<style scoped>
.between-cards {
  padding: 2rem, 4rem;
}
</style>
