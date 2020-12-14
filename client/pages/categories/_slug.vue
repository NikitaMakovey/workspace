<template>
  <div>
    <h1>{{ $route.params.slug }}</h1>
    <list :cards="books"></list>
  </div>
</template>

<script>
import List from "../../components/IndexComponents/List";

export default {
  name: "_slug",
  components: {
    List
  },
  data() {
    return {
      books: [
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 5 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 5 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 5 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 5 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 5 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 5 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 5 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 5 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 5 },
      ]
    }
  },
}
</script>

<style scoped>

</style>
