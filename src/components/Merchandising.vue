<template>
  <section class="merchandising">
    <div class="container">
      <div class="merch-list" v-for="(merch, index) in merchType" :key="index">
        <img :src="'../assets7img7buy-comics-' + merch.image" alt=""><span>{{merch.name}}</span>
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
          image: "digital-comics.png",
          url: "adsadssda"
        },
        {
          name: "DC MERCHANDISE",
          image: "merchandise.png",
          url: "adsadssda"
        },
        {
          name: "SUBSCRIPTION",
          image: "shop-locator.png",
          url: "adsadssda"
        },
        {
          name: "COMIC SHOP LOCATOR",
          image: "subscriptions.png",
          url: "adsadssda"
        },
        {
          name: "DC POWER VISA",
          image: "subscriptions.png",
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
    }
  }
  
</style>