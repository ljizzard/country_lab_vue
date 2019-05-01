<template lang="html">
<div>
  <ul>
    <list-item v-for="(country, index) in countries" :country="country" :key="index"></list-item>
  </ul>

</div>
</template>

<script>
import listItem from './listItem.vue';

export default {
  name: 'country-list',
  props: ['countries'],
  components: {
    "list-item": listItem
  }
}
</script>

<style lang="css" scoped>
</style>
