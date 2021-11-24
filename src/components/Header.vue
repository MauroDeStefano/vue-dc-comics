<template>
  <header class="container">
    <div>
      <img src="../assets/img/dc-logo.png" alt="">
    </div>
      <nav>
        <a v-for="(item, index) in navBtn" :key="index" @click="item.active = !item.active" :class="{active: item.active}" >{{item.name}}</a>
      </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
  data(){
    return{
      navBtn:[
        {
          name: "CHARACTERS",
          active: false,
          url: "prova"
        },
        {
          name: "COMICS",
          active: true,
          url: "prova"
        },
        {
          name: "MOVIES",
          active: false,
          url: "prova"
        },
        {
          name: "TV",
          active: false,
          url: "prova"
        },
        {
          name: "GAMES",
          active: false,
          url: "prova"
        },
        {
          name: "COLLECTIBLES",
          active: false,
          url: "prova"
        },
        {
          name: "VIDEOS",
          active: false,
          url: "prova"
        },
        {
          name: "FANS",
          active: false,
          url: "prova"
        },
        {
          name: "NEWS",
          active: false,
          url: "prova"
        },
        {
          name: "SHOP",
          active: false,
          url: "prova"
        }
      ]
    }
  }
}

</script>

<style lang="scss">
  header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 150px;


    nav{
      
      a{
        float: left;
        margin-left: 20px;
        text-decoration: none;
        color: black;
        line-height: 145px;
        border-bottom: 5px solid white;
        
      }
      .active{
        color: #0C7CEC;
        border-bottom: 5px solid #0C7CEC;
      }
    }
  }
</style>