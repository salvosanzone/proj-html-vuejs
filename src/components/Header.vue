<template>

  <header>
    <div class="top-header d-flex justify-content-center align-items-center">
      <div class="container">
        <div>
          <a class="" href="">
            <i class="fas fa-phone me-2"></i>
          </a>
          <span>Call us for a Free Quote 1.800.555.67.89</span>
        </div>
        <div>
          <i class="fab fa-facebook-f me-3"></i>
          <i class="fab fa-twitter me-3"></i>
          <i class="fab fa-instagram me-3"></i>
          <i class="fab fa-youtube me-3"></i>
        </div>
      </div>
    </div>
    <div class="bottom-header">
       <div class="container">
        <div class="row align-items-baseline">
          <div class="col-1">
            <div class="logo">
              <img src="../assets/img/avada-movers-logo.png" alt="" />
            </div>
          </div>
          <div class="col-11 d-flex justify-content-end">
            <div class="menu">
              <ul class="d-flex justify-content-center align-items-center">
                <li>
                  <a href=""> <strong> Home </strong> </a>
                </li>
                <li>
                  <a href=""> <strong> Rates </strong> </a>
                </li>
                <li>
                  <a href=""> <strong> Testimonials </strong> </a>
                </li>
                <li>
                  <a href=""> <strong> FAQ </strong> </a>
                </li>
                <li>
                  <a href=""> <strong> Blog </strong> </a>
                </li>
                <li>
                  <a href=""> <strong> Contact </strong> </a>
                </li>
                
                <li>
                  <a href="">
                    <button class="btn-small"> <strong> FREE QUOTE </strong> </button>
                  </a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div> 
      <div class="center-container d-flex flex-column align-items-center">
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
};
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";
@import "../assets/style/mixins.scss";
@import "../assets/style/general.scss";

header {
  .top-header {
    height: 30px;
    background-color: $lima;
    color: white;
    .container {
      @include flex("between");
      //border: 1px solid black;
      a {
        color: white;
      }
    }
  }
  .bottom-header {
    height: 535px;
    padding: 10px;
    background-image: url(../assets/img/avada-movers-homeherobackground-final.jpg);
    @include background("");
    .container {
      margin-bottom: 150px;
      .logo {
        width: 120px;
      }
      ul li {
        list-style: none;
        margin: 0 5px;

        a {
          text-decoration: none;
          margin: 0 12px;
          color: black;
        }
      }
    }
    .center-container {
      margin: 0 auto;
      span{
        color: $oslo-gray;
      }
    }
  }
}
</style>