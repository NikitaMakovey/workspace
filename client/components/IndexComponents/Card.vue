<template>
  <div class="col-sm-6 col-md-6 col-lg-4 col-xl-3 col-6 card-container">
    <div class="card" style="width: 18rem;">
      <img :src="item.image" class="card-img-top" alt="#">
      <div class="card-body">
        <p class="card-text">{{ item.title }}</p>
        <div style="display: block; width: 100%">
          <div style="display: inline-block; margin: 0 auto; float: left;"><p class="card-text card-price">{{ item.price }} $</p></div>
          <div style="display: inline-block; float: right"><button class="btn btn-primary">Buy</button></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: [ 'item' ]
}
</script>

<style scoped>
  .card-container {
    margin: 0.5rem 0.2rem;
  }
  .card-price {
    font-size: 1.5rem;
  }
</style>
