<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse">
      <ul class="navbar-nav">
        <template v-for="category in categories">
          <li class="nav-item">
            <nuxt-link
              class="nav-link" :to="`/categories/${category.slug}`"
              role="button" aria-haspopup="true" aria-expanded="false"
            >
              {{ category.name }}
            </nuxt-link>
          </li>
        </template>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  props: ['categories'],
  methods: {
    getCategory(slug) {
      return this.categories.filter(category => category.slug === slug).name
    }
  }
}
</script>

<style scoped>

</style>
