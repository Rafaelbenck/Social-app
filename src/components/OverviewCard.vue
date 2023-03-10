<template>
  <v-card class="mx-auto" variant="outlined" style="margin: 2rem 0">
    <v-card-item>
      <div>
        <div class="text-overline mb-1">
          <v-avatar class="avatar-margin" color="grey-darken-1" size="32"></v-avatar>OVERLINE
        </div>
        <div class="text-h6 mb-1">Headline</div>
        <div class="text-caption">Greyhound divisely hello coldly fonwderfully</div>
      </div>
    </v-card-item>

    <btnShowMore />
    <br />

    <v-row justify="space-around">
      <v-col cols="auto">
        <v-sheet>
          <v-chip-group multiple selected-class="text-primary" style="margin: 0.3rem">
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
import btnShowMore from './btnShowMore.vue'
export default {
  name: 'OverviewCard',
  components: { btnShowMore },
  data: () => ({
    tags: ['Best seller', 'Most view', 'Other text']
  })
}
</script>

<style scoped>
.between-cards {
  padding: 2rem, 4rem;
}

.avatar-margin {
  margin-right: 0.7rem;
}
</style>
