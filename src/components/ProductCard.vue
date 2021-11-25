<template>
  <div class="product-card">
    <div class="card">
      <img :src="product.thumb" :alt="product.series">
      <h3>{{product.series}}</h3>
    </div>
  </div>
</template>

<script>

export default {

  name: 'ProductCard',
  props:{
    product: Object,
  }
}

</script>


<style lang="scss">


.product-card{
  display: flex;
  flex-wrap: wrap;
  width: calc(100% / 6);

  .card{
    display: inline-block;
    padding-bottom: 20px;
  }
  img{
    width: 150px;
    height: 150px;
    object-fit: cover;
    object-position: top;
    
  }
}

</style>