<template lang="html">
  <ul>
    <list-item v-for="(country, index) in countries" v-bind:country="country" v-bind:key="index"></list-item>
  </ul>
</template>

<script>
  import ListItem from "./ListItem.vue";

  export default {
    name: 'countries-list',
    props: ['countries'],
    components: {
      "list-item": ListItem
    }
  }
</script>

<style lang="css" scoped>
</style>
