<template>
  <footer>
    <div class="footer-top">
      <div class="container">
        <div class="link-list">
          <div v-for="(list, index) in listLinks" :key="`list${index}`">
            <h2>{{list.name}}</h2>
            <ul>
              <li v-for="(underList, i) in list.links" :key="`underList${i}`">
                {{underList.name}}
              </li>
            </ul>
          </div>
        </div>
        <div class="dc-logo">
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <div class="container">
        <div class="sign">
          <button>SIGN-UP NOW!</button>
        </div>
        <div class="social">
          <div> FOLLOW US </div>
          <div></div>
        </div>
      </div>  
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data(){
    return{
      listLinks:[
        {
          name: "DC COMICS",
          links:[
            {
              name: "Characters",
              url: "example.com"
            },
            {
              name: "Comics",
              url: "example.com"
            },
            {
              name: "Movies",
              url: "example.com"
            },
            {
              name: "TV",
              url: "example.com"
            },
            {
              name: "Games",
              url: "example.com"
            },
            {
              name: "Videos",
              url: "example.com"
            },
            {
              name: "News",
              url: "example.com"
            }
          ]
        },
        {
          name: "SHOP",
          links:[
            {
              name: "Shop DC",
              url: "example.com"
            },
            {
              name: "Shop DC Collectibles",
              url: "example.com"
            }
          ]
        },
        {
          name: "DC",
          links:[
            {
              name: "Terms Of Use",
              url: "example.com"
            },
            {
              name: "Privacy policy (New)",
              url: "example.com"
            },
            {
              name: "Ad Choices",
              url: "example.com"
            },
            {
              name: "Advertising",
              url: "example.com"
            },
            {
              name: "Jobs",
              url: "example.com"
            },
            {
              name: "Subscriptions",
              url: "example.com"
            },
            {
              name: "Talent Workshopd",
              url: "example.com"
            },
            {
              name: "CPSC Certificates",
              url: "example.com"
            },
            {
              name: "Ratings",
              url: "example.com"
            },
            {
              name: "Shop Help",
              url: "example.com"
            },
            {
              name: "Contact Us",
              url: "example.com"
            }
          ]
        },
        {
          name: "SITES",
          links:[
            {
              name: "DC",
              url: "example.com"
            },
            {
              name: "MAD Magazine",
              url: "example.com"
            },
            {
              name: "DC Kids",
              url: "example.com"
            },
            {
              name: "DC Universe",
              url: "example.com"
            },
            {
              name: "DC Power Visa",
              url: "example.com"
            }
          ]
        }
      ]
    }
  }
}
</script>

<style lang="scss">

.footer-top{
  display: flex;
  background-image: url("../assets/img/footer-bg.jpg");
  background-size: cover;
  height: 450px;
  .link-list{
    float: left;
    width: 50%;
    height: 100%;
    padding: 60px 0;
    color: white;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    
    h2{
      padding-left: 10px ;
    }
    ul{
      padding: 10px;
      li{
        list-style: none;
        color: gray;
      }
    }
  }
  .dc-logo{
    float: left;
    width: 50%;
    height: 100%;
    background-image: url("../assets/img/dc-logo-bg.png");
    background-position: center;
    background-size: cover ;
  }

}


.footer-bottom{
  width: 100%;
  height: 100px;
  background-color: #303030;
  display: flex;
  align-items: center;
  
  .container{
    display: flex;
    justify-content: space-between;

    .sign{
      color: white;
    }
    .social{  
      color: #0087FF;
    }
  } 
}
</style>