<template>
  <div class="header-container">
      <div class="container pt-4 d-flex justify-content-between align-items-center">
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
  .container{
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