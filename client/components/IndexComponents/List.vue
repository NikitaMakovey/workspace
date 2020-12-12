<template>
  <div class="row">
    <template v-for="card in cards">
      <Card :item="card"></Card>
    </template>
  </div>
</template>

<script>
import Card from "./Card";

export default {
  name: "List",
  props: [ 'cards' ],
  components: {
    Card
  }
}
</script>

<style scoped>

</style>
