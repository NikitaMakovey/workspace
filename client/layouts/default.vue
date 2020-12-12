<template>
  <div>
    <navbar></navbar>
    <search-navbar></search-navbar>
    <category-list :categories="categories"></category-list>
    <div class="container">
      <nuxt />
    </div>
    <footer-container></footer-container>
  </div>
</template>

<script>
import Navbar from "../components/Navbar";
import SearchNavbar from "../components/SearchNavbar";
import CategoryList from "../components/CategoryList";
import FooterContainer from "../components/Footer";

export default {
  data() {
    return {
      categories: [
        {
          name: 'CategoryName', items: [
            { name: 'CategoryName', link: 'category-link' },
            { name: 'CategoryName', link: 'category-link' },
            { name: 'CategoryName', link: 'category-link' },
            { name: 'CategoryName', link: 'category-link' },
          ]
        },
        {
          name: 'CategoryName', items: [
            { name: 'CategoryName', link: 'category-link' },
            { name: 'CategoryName', link: 'category-link' },
            { name: 'CategoryName', link: 'category-link' },
            { name: 'CategoryName', link: 'category-link' },
          ]
        },
        {
          name: 'CategoryName', items: [
            { name: 'CategoryName', link: 'category-link' },
            { name: 'CategoryName', link: 'category-link' },
            { name: 'CategoryName', link: 'category-link' },
            { name: 'CategoryName', link: 'category-link' },
          ]
        },
        {
          name: 'CategoryName', items: [
            { name: 'CategoryName', link: 'category-link' },
            { name: 'CategoryName', link: 'category-link' },
            { name: 'CategoryName', link: 'category-link' },
            { name: 'CategoryName', link: 'category-link' },
          ]
        },
        {
          name: 'CategoryName', items: [
            { name: 'CategoryName', link: 'category-link' },
            { name: 'CategoryName', link: 'category-link' },
            { name: 'CategoryName', link: 'category-link' },
            { name: 'CategoryName', link: 'category-link' },
          ]
        },
      ],
    }
  },
  components: {
    FooterContainer,
    Navbar,
    SearchNavbar,
    CategoryList
  }
}
</script>

<style>

</style>
