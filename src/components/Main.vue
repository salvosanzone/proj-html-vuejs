<template>

  <main>
    <section class="get-free-quote">
      <div class="center-container align-items-center">
          <i class="fab fa-telegram-plane me-3"></i>
        <span>GET A FREE QUOTE ONLINE NOW!</span>
      </div>
    </section>
    <section class="award-winning">
      <div class="center-container">
        award winning
      </div>
    </section>
    <section class="full-service">
      <div class="center-container">
        full service
      </div>
      <div class="container">
        column
      </div>
    </section>
    <section class="move-with-ease">
      move whith ease
    </section>
    <section class="testimonials">
      <div class="center-container">
        testimonials
      </div>
      <div class="container">
        column
      </div>
    </section>
    <section class="request-free-quote">
      <div class="center-container">
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
      background-color: $denim;
      @include flex('center');
      span{
        color: white;
        font-size: 12px;

      }
    }
    .award-winning{
      height: 445px;
      background-image: linear-gradient(white, $mercury);
    }
    .full-service{
      height: 670px;
      border: 1px solid black;
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