<template>
  <v-container>
    <HelloWorld />
    <Contents />
  </v-container>
</template>

<script lang="ts">
import Vue from "vue";
import HelloWorld from "../components/HelloWorld.vue";
import Contents from "../components/Contents.vue";

export default Vue.extend({
  components: {
    HelloWorld,
    Contents
  }
});
</script>
