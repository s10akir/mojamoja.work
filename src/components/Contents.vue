<template>
  <v-container>
    <v-layout text-center wrap>
      <v-flex xs12>
        <v-btn
          v-for="link in links"
          :key="link.id"
          class="my-4"
          outlined
          block
          x-large
          :href="link.href"
          target="_blank"
        >
          {{ link.title }}
        </v-btn>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  data: () => ({
    links: [
      {
        title: "Portfolio",
        href: "https://portfolio.mojamoja.work"
      },
      {
        title: "Github",
        href: "https://github.com/s10akir"
      },
      {
        title: "Twitter",
        href: "https://twitter.com/s10akir"
      }
    ]
  })
});
</script>
