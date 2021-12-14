<template>

  <header>
    <div class="top-header">
      <div class="big-container">
        <div>
          <a class="" href="">
            <i class="fas fa-phone me-2"></i>
          </a>
          <span>Call us for a Free Quote 1.800.555.67.89</span>
        </div>
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
    <div class="bottom-header d-flex align-items-center flex-column">
      <div class="menu-bottom-header big-container">
        <div class="row align-items-baseline">
          <div class="col-1">
            <div class="logo">
              <img src="../assets/img/avada-movers-logo.png" alt="" />
            </div>
          </div>
          <div class="col-11 d-flex justify-content-end">
            <div class="menu">
              <ul class="d-flex justify-content-center align-items-center">
                <li 
                  v-for="item in menu" 
                  :key="item.id"
                >
                  <a 
                    :class="{active: item.actived === true}"
                    @click="item.actived = !item.actived" 
                    :href="item.name"
                  >
                    {{item.name}}
                  </a>
                </li>
                <li>
                  <a href="">
                    <button class="btn-small">  FREE QUOTE </button>
                  </a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
      <div class="text-bottom-header small-container">
          <span>MOVING WITHOUT THE HASSLE</span>
          <h2>WE MAKE IT SIMPLE</h2>
          <span>PROFESSIONAL SERVICE WITH QUALITY AND CUSTOMER SATISFATION</span>
      </div>
    </div>
  </header>

</template>

<script>
export default {
  name: "Header",
  //Header riceve da App un array tramite la props
  props:{
    menu: Array
  }
};
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";
@import "../assets/style/mixins.scss";
@import "../assets/style/general.scss";

header {
  .top-header {
    height: 30px;
    @include flex('center');
    background-color: $lima;
    color: white;
    .big-container {
      @include flex("between");
      a {
        color: $white;
      }
      
    }
  }
  .bottom-header {
    height: 535px;
    padding: 10px;
    background-image: url(../assets/img/avada-movers-homeherobackground-final.jpg);
    @include background("");
    background-size: 125%;
    position: relative;
    .menu-bottom-header{
      .logo{
        width: 120px;
      }
      a{
        color: $black;
        font-weight: 800;
      }
      a.active{
       color: $mantis !important;
      }
    }
    .text-bottom-header{
      position: absolute;
      top: 50%;
      span{
        color: $river-bed;
        font-weight: 800;
      }
      h2{
        font-weight: 800;
        font-size: 40px;
      }
    }
    
  }
}
</style>