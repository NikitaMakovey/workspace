<template>
  <div>
    <div class="row">
      <div class="col-12">
        <list :cards="books"></list>
      </div>
    </div>
  </div>
</template>

<script>
import List from "../components/IndexComponents/List";

export default {
  data() {
    return {
      books: [
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 20 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 20 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 20 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 20 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 20 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 20 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 20 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 20 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 20 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 20 },
        { image: require(`~/assets/book.jpg`), title: 'BookTitle', price: 20 },
      ]
    }
  },
  components: {
    List
  }
}
</script>

<style>

</style>
