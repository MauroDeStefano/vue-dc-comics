<template>
  <main>
    <span class="container current ">CURRENT SERIES</span>
    <div class="container cards">
      <ProductCard v-for="(product, index) in productsList" :key="index" :product="product" />
    </div>
  </main>
</template>

<script>

import ProductCard from "./ProductCard.vue";
import productsList from "../assets/data/productsList.js"

export default {
  name: "Main",
  components:{
    ProductCard
  },
  data(){
   return{
     productsList
   }
  },

}



</script>

<style lang="scss">
 
 main{
  position: relative;
  background-color: #1C1C1C;
  color: white;
  display: flex;
  align-items: center;

  .current{
    display: flex;
    text-align: center;
    justify-content: center;
    align-items: center;
    position: absolute;
    width: 200px;
    height: 50px;
    top: -20px;
    left: 330px;
    background-color: #0C7CEC;
  }

  .cards{ 
    margin-top: 50px;
    margin-bottom: 50px;
    display: flex;
    flex-wrap: wrap;
  }
 }
</style>