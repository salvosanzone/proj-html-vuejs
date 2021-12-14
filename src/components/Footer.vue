<template>

  <footer>
    <div class="top-footer">
      <div class="container">
        <div class="small-container align-items-start me-5 justify-content-around">
          <span>ABOUT</span>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod amet repellat vero placeat fugit et commodi nulla exercitationem excepturi, officiis ullam explicabo quo voluptas, accusantium quos illum veritatis harum in.</p>
          <div class="logo-footer">
            <img src="../assets/img/avada-movers-retinalogo.png" alt="">
          </div>
        </div>
        <div class="small-container align-items-start justify-content-around">
          <span>AVADA MOVERS</span>
          <span><i class="fas fa-chevron-right"></i><a href="">Home</a></span>
          <span><i class="fas fa-chevron-right"></i> <a href="">Rates</a> </span>
          <span><i class="fas fa-chevron-right"></i> <a href="">Testimonials</a></span>
          <span><i class="fas fa-chevron-right"></i> <a href="">Blog</a></span>
          <span><i class="fas fa-chevron-right"></i> <a href="">Free Quote</a></span>
          
        </div>
        <div class="small-container align-items-start justify-content-around">
          <span>RECENT POSTS</span>
          <span><i class="fas fa-chevron-right"></i> <a href="">Heading Out To College?</a></span>
          <span><i class="fas fa-chevron-right"></i> <a href="">Moving Your Business?</a></span>
          <span><i class="fas fa-chevron-right"></i> <a href="">Outstanding Quality</a></span>
          <span><i class="fas fa-chevron-right"></i> <a href="">Cost Of Moving</a></span>
          <span><i class="fas fa-chevron-right"></i> <a href="">Best Moving Tips</a></span>
          
        </div>
        
      </div>
    </div>
    <div class="bottom-footer">
      <div class="small-container">
        <i class="far fa-copyright my-3"> Copyright 2012 - 2020 | Avada Theme by ThemeFusion | All Rights Reserved | Powered by WordPress</i>
        <div>
          <a href="">
            <i class="fab fa-facebook-f me-3"></i>
          </a>
          <a href="">
            <i class="fab fa-twitter me-3"></i>
          </a>
          <a href="">
            <i class="fab fa-instagram me-3"></i>
          </a>
          <a href="">
            <i class="fab fa-youtube me-3"></i>
          </a>
        </div>
      </div>
    </div>
  </footer>

</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";
@import '../assets/style/mixins.scss';

  footer{
    .top-footer{
      @include flex('center');
      height: 300px;
      border-top: 10px solid $lima;
      .container{
        @include flex('');
        .logo-footer{
          width: 120px;
        }
        i, a{
          color: $black;
        }


      }
    }
    .bottom-footer{
      @include flex('center');
      height: 95px;
      background-color: $lima;
      
    }
  }

</style>