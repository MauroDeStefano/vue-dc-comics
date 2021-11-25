<template>
  <section class="merchandising">
    <div class="container">
      <div class="merch-list" v-for="(merch, index) in merchType" :key="index">
        <img :src="merch.image" alt=""><span>{{merch.name}}</span>
      </div>
    </div>
  </section>
</template>

<script>


export default {
  name: "Merchandising",
  data(){
    return{
      merchType:[
        {
          name: "DIGITAL COMICS",
          image: require("../assets/img/buy-comics-digital-comics.png"),
          url: "adsadssda"
        },
        {
          name: "DC MERCHANDISE",
          image: require("../assets/img/buy-comics-merchandise.png"),
          url: "adsadssda"
        },
        {
          name: "SUBSCRIPTION",
          image: require("../assets/img/buy-comics-subscriptions.png"),
          url: "adsadssda"
        },
        {
          name: "COMIC SHOP LOCATOR",
          image: require("../assets/img/buy-comics-shop-locator.png"),
          url: "adsadssda"
        },
        {
          name: "DC POWER VISA",
          image: require("../assets/img/buy-dc-power-visa.svg"),
          url: "adsadssda"
        },
      ]
    }
  }
}
</script>

<style lang="scss">
  .merchandising{
    height: 150px;
    width: 100%;
    background-color:#0282F9;
    display: flex;
    align-items: center;
    vertical-align: middle;
    justify-content: center;

    div{
      display: flex;
      justify-content: space-between;
      align-items: center;
      color: white;
      &:hover{
        cursor: pointer;
      }

      img{
        width: 40px;
        margin-right: 10px;
      }
    }
  }
  
</style>