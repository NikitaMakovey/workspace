<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavDropdown">
      <ul class="navbar-nav">
        <template v-for="(category, i) in categories">
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle" href="#" :id="`navbarDropdownMenuLink${i}`"
              role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false"
            >
              {{ category.name }}
            </a>
            <div class="dropdown-menu" :aria-labelledby="`navbarDropdownMenuLink${i}`" v-if="category.items.length > 0">
              <template v-for="item in category.items">
                <a class="dropdown-item" :href="`/categories/${item.link}`">{{ item.name }}</a>
              </template>
            </div>
          </li>
        </template>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  props: ['categories']
}
</script>

<style scoped>

</style>
