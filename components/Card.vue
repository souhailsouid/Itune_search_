<template>
  <div id="e3" style="max-width: 400px; margin: auto;" class="grey lighten-3">
    <v-container fluid style="min-height: 0" grid-list-lg>
      <v-layout row wrap>
        <v-flex xs12>
          <v-card target="_blank" :href="url" :color="color" class="white--text">
            <v-layout row>
              <v-flex xs7>
                <v-card-title primary-title>
                  <div>
                    <div class="headline">{{title}}</div>
                    <div>{{artistName}}</div>
                  </div>
                </v-card-title>
              </v-flex>
              <v-flex xs5>
                <v-img :src="image" height="125px" contain></v-img>
              </v-flex>
            </v-layout>
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
  </div>
</template>

<script>
export default {
  props: ["title", "image", "artistName", "url", "color"]
};
</script>
<style>
</style>