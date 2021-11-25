<template>
  <main>
    <div class="container current ">
      <span>CURRENT SERIES</span> 
    </div>
    <div class="container cards">
      <ProductCard v-for="(product, index) in productsList" :key="index" :product="product" />
    </div>
    <div class="container load">
      <span>LOAD MORE</span> 
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
  background-color: #1C1C1C;
  color: white;
  padding-bottom: 20px;


  .current{
  position: relative;

  span{    
    display: flex;
    text-align: center;
    justify-content: center;
    align-items: center;
    position:absolute;
    top: -25px;
    left: 0px;  
    width: 200px;
    height: 50px;
    background-color: #0C7CEC;

     &:hover{
      cursor: pointer;
    }
  }
  }

  .cards{ 
    padding-top: 50px;
    padding-bottom: 50px;
    display: flex;
    flex-wrap: wrap;

     &:hover{
      cursor: pointer;
    }
  }
  .load{
    display: flex;
    text-align: center;
    justify-content: center;
    align-items: center;
    width: 200px;
    height: 50px;
    background-color: #0C7CEC;

    &:hover{
      cursor: pointer;
    }
  }
 }

</style>