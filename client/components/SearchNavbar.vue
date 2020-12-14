<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarTogglerDemo01">
      <nuxt-link class="navbar-brand" to="/"><img :src="require(`~/assets/logo.svg`)" alt="#" style="max-height: 80px"></nuxt-link>
      <form class="form-inline my-2 my-lg-0" style="margin: 0 auto">
        <input class="form-control mr-sm-2" type="search" placeholder="Search" style="min-width: 30rem; min-height: 3rem" aria-label="Write something and search...">
        <button class="btn btn-outline-success my-2 my-sm-0" style="min-height: 3rem" type="submit">Search</button>
      </form>
      <a class="navbar-brand" href="#"><img :src="require(`~/assets/cart.png`)" alt="#" style="max-height: 40px;"></a>
    </div>
  </nav>
</template>

<script>
export default {

}
</script>

<style scoped>

</style>
