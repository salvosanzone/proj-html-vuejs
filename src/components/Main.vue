<template>

  <main>
    <section class="get-free-quote">
      <div class="small-container flex-row">
        <a href="">
          <i class="fab fa-telegram-plane me-3"></i>
        </a>
        <span>GET A FREE QUOTE ONLINE NOW!</span>
      </div>
    </section>
    <section class="award-winning">
      <div class="small-container">
        <span>HEADACHE FREE</span>
        <h2>Award Winning</h2>
        <h2>Moving Company</h2>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta in illo earum aspernatur pariatur ea iste nihil officia ipsam veritatis. Necessitatibus non temporibus iure fugiat officiis rem inventore natus iste.</p>
        <button class="btn-big">REAR OUR TESTIMONIALS</button>
      </div>
    </section>
    <section class="full-service">
      <div class="small-container">
        <span>WE ARE A PROFESSIONAL</span>
        <h2>Full-Service Solution</h2>
      </div>
      <div class="container">
        <div class="card">
          <div class="pic-card d-flex justify-content-center">
            <img src="../assets/img/avada-movers-serviceonephoto-final-400x255.jpg" alt="">
          </div>
          <div class="text-card text-center">
            <h5>Two Man Teams</h5>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas debitis aspernatur odio suscipit asperiores eaque unde, minus repellendus eveniet repellat dicta perferendis? Eaque architecto doloremque incidunt assumenda vel necessitatibus ipsam.</p>
            <button class="btn-small">READ MORE</button>
          </div>
        </div>
        <div class="card">
          <div class="pic-card d-flex justify-content-center">
            <img src="../assets/img/avada-movers-servicetwophoto-final-400x255.jpg" alt="">
          </div>
          <div class="text-card text-center">
            <h5>Two Man Teams</h5>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas debitis aspernatur odio suscipit asperiores eaque unde, minus repellendus eveniet repellat dicta perferendis? Eaque architecto doloremque incidunt assumenda vel necessitatibus ipsam.</p>
            <button class="btn-small">READ MORE</button>
          </div>
        </div>
        <div class="card">
          <div class="pic-card d-flex justify-content-center">
            <img src="../assets/img/avada-movers-servicethreephoto-final-400x255.jpg" alt="">
          </div>
          <div class="text-card text-center">
            <h5>Two Man Teams</h5>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas debitis aspernatur odio suscipit asperiores eaque unde, minus repellendus eveniet repellat dicta perferendis? Eaque architecto doloremque incidunt assumenda vel necessitatibus ipsam.</p>
            <button class="btn-small">READ MORE</button>
          </div>
        </div>
      </div>
    </section>
    <section class="move-with-ease">
      move whith ease
    </section>
    <section class="testimonials">
      <div class="small-container">
        testimonials
      </div>
      <div class="container">
        column
      </div>
    </section>
    <section class="request-free-quote">
      <div class="small-container">
        request a free quote
      </div>
    </section>
  </main>

</template>

<script>
export default {
  name: 'Main'
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";
@import '../assets/style/mixins.scss';

  main{
    .get-free-quote{
      height: 100px;
      background-color: $denim-vibrant;
      //@include flex('center');
      a{
        color: $white;
      }
      span{
        color: $white;
        font-size: 12px;

      }
    }
    .award-winning{
      height: 445px;
      background-image: linear-gradient(white, $mercury);
      //@include flex('center');
    }
    .full-service{
      height: 670px;
      .small-container{
      }
      .container{
        @include flex('');
        .card{
          display: flex;
          justify-content: space-between;
          width: calc(100% / 3 - 20px);
          height: 370px;
          margin: 0 20px;
          padding: 15px;
          background-color: $mercury;
        }
        .text-card{
          padding: 5px;
          background-color: $white;
        }

      }
    }
    .move-with-ease{
      height: 535px;
      background-image: url(../assets/img/avada-movers-movewithease-background-new.jpg);
      @include background('');
    }
    .testimonials{
      height: 670px;
      background-image: url(../assets/img/avada-movers-testimonial-background.jpg);
      @include background('');
      
    }
    .request-free-quote{
      height: 370px;
      background-image: url(../assets/img/avada-movers-request-quote-background.jpg);
      @include background('');

    }
  }
</style>