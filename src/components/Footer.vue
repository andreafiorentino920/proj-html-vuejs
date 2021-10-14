<template>
  <div class="footer">
      <div class="footer-top">
        <div class="container d-flex justify-content-center">
          <div class="row">
            <div class="col-3">
              <h5>COME TO FIND US</h5>
              <ul>
                <li :key="index" v-for="(link,index) in menu1">
                {{link.text}}
                </li>
              </ul>
              
            </div>
            <div class="col-3">
              <h5>RECENT POST</h5>
              <ul>
                <li :key="index" v-for="(link,index) in menu2">
                {{link.text}}
                </li>
              </ul>
            </div>
            <div class="col-3">
              <h5>COME TO FIND US</h5>
              <ul>
                <li :key="index" v-for="(link,index) in menu3">
                {{link.text}} <br>
                {{link.time}}
                </li>
              </ul>
            </div>
            <div class="col-3">
              <img :src="'../assets/images/' + foto.link" alt="">
            </div>
          </div>
        </div>
      </div>
      <div class="footer-bottom">
        <div class="container">
          <div class="row">
            <div class="col-8">
              <ul class="d-flex flex-row">
                <li v-for="(link,index) in menu4" :key="index">
                  {{link.text}}
                </li>
              </ul>
            </div>
            <div class="col-4 d-flex align-items-center">
              <div class="row">
                <div class="icon d-flex justify-content-center align-items-center" :key="index" v-for="(icon,index) in icons">
                <i :class="[icon.class]"></i>
              </div>
              </div>
              
            </div>
          </div>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name:"Footer",
    data(){
      return{
        menu1:[
        {
          text:"12345 North Main Street"
        },
        {
          text:"New York, NY 555555"
        },
        {
          text:"Phone: 1.800.555.6789"
        },
        {
          text:"Email:info@your-domain.com"
        }
      ],
      menu2:[
        {
          text:"Train with free weights or your body weight?"
        },
        {
          text:"Nutritional advice thath will keep your training"
        }
      ],
      menu3:[
        {
          text:"Weekdays Monday-Friday",
          time:"09:00 - 19:00"
        },
        {
          text:"Weekends Saturday-Sunday",
          time:"09:00 - 21:00"
        }
      ],
      foto:{
        link:"gym_ad-compressor.jpg"
      },
      menu4:[
        {
          text:"Copyright 2012 - 2020"
        },
        {
          text:"Awada Theme by Theme Fusion"
        },
        {
          text:"All Rights Reserved"
        },
        {
          text:"Powered by Wordpress"
        }
      ],
      icons:[
        {
          class:"fab fa-facebook-f"
        },
        {
          class:"fab fa-twitter"
        },
        {
          class:"fab fa-instagram"
        }
      ]
    }
  }    
}
</script>

<style lang="scss">
.footer{
  h5{
      color: #3d4245;
    }
    ul{
      list-style-type: none;
      li{
      color: #999999;
    }
    }
  .footer-top{
    background-color: #1f2123;
  }
  .footer-bottom{
    background-color: #1a1c1e;
    .container{
      .row{
        .icon:nth-child(2){
          margin: 0 10px ;
        }
        .icon{
          font-size: 25px;
          color: white;
          width: 50px;
          height: 50px;
          background-color: #d5645e;
        }
      }
    }
  }
}
</style>