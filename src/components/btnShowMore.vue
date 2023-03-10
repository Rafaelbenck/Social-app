<template>
  <v-layout style="height: 128px">
    <div class="mx-auto my-4">
      <v-expansion-panels @click.active:="active = !active" class="border rounded">
        <v-expansion-panel
          title="Show More"
          text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, ratione debitis quis est labore voluptatibus! Eaque cupiditate minima"
        >
        </v-expansion-panel>
      </v-expansion-panels>
    </div>

    <v-bottom-navigation :active="active" color="ligth-grey" border-radius="70px">
      <v-btn>
        <v-icon>mdi-history</v-icon>

        Recents
      </v-btn>

      <v-btn>
        <v-icon>mdi-heart</v-icon>

        Favorites
      </v-btn>

      <v-btn>
        <v-icon>mdi-map-marker</v-icon>

        Nearby
      </v-btn>
    </v-bottom-navigation>
  </v-layout>
</template>

<script>
export default {
  data: () => ({ active: true })
}
</script>
