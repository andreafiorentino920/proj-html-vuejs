<template>
  <div class="header-container">
      <div class="container container-menu pt-5 d-flex justify-content-between align-items-center">
        <div class="logo">
        </div>
        <div class="menu">
          <ul class="d-flex flex-row">
            <li>
              <a class="selected" href="#">HOME</a>
            </li>
            <li>
              <a href="#">ABOUT US </a>
            </li>
            <li>
              <a href="#">FACILITIES </a>
            </li>
            <li>
              <a href="#">MEMBERSHIP </a>
            </li>
            <li>
              <a href="#">TESTIMONIALS</a>
            </li>
            <li>
              <a href="#">BLOG</a>
            </li>
          </ul>
        </div>
      </div>
      <div class="d-flex justify-content-center">
        <div class="container-hero d-flex flex-column align-items-center">
        <h1>NO PAIN NO GAIN</h1>
        <p>Motivation is what gets you started. Habit is what keeps you going</p>
        <button>JOIN US TODAY</button>
      </div>
      </div>
      
  </div>
</template>

<script>
export default {
    name:"Header"
}
</script>

<style lang="scss" >
.header-container{
  background-image: url("../assets/images/home-banner.jpg");
  background-size:cover; 
  height: 800px;

  .container-hero{
    margin-top: 170px;
    h1{
      font-size: 100px;
      color: white;
    }
    p{
      font-size: 20px;
      color: white;
    }

    button{
      background-color: transparent;
      padding: 10px 20px 10px 20px;
      color: #a7a6a5;
      border: #a7a6a5 solid 2px;
    }
  }

  .container-menu{
      .logo{
      background-image: url("../assets/images/gym_logo_1x.png");
      width: 250px;
      height: 100px;
      }
      .menu{
        .selected{
          color: #ee6059;
        }
        ul{
          li{
          list-style-type: none;
          margin-left: 30px;
          a{
          color: white;
          text-decoration: none;
          }
          }
        }
      }
      
  }
  
 
}

</style>