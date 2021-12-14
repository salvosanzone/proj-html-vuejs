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
      <div class="container">
        <div class="content flex-column">
          <span>WE REMOVE THE HEADACHE FROM MOVING</span>
          <h2>Move with Ease</h2>
          <p>With our super simple service we can take you from getting a quote, right throught to being in your new home with all of your belongings securely packed and safely delivered, even in the rooms of your choice.</p>
          <button class="btn-big">GET A FREE QUOTE NOW</button>
        </div>
      </div>
    </section>
    <section class="testimonials">
      <div class="small-container">
        <span>HAPPY CUSTOMERS</span>
        <h2>Testimonials</h2>
      </div>
      <div class="container my-5">
        <div class="small-container mx-5">
          <div class="testimonial-pic">
            <img src="../assets/img/avada-movers-johndoe-final-200x200.jpg" alt="">
          </div>
          <h4>John Doe</h4>
          <p class="text-center">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptatem ut accusantium deserunt esse sapiente consequuntur aperiam architecto assumenda ullam minima soluta voluptas recusandae excepturi, ducimus repudiandae? Vitae maiores suscipit eaque?</p>
        </div>
        <div class="small-container mx-5">
          <div class="testimonial-pic">
            <img src="../assets/img/avada-movers-janedoe-final-200x200.jpg" alt="">
          </div>
          <h4>Jane Doe</h4>
          <p class="text-center">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptatem ut accusantium deserunt esse sapiente consequuntur aperiam architecto assumenda ullam minima soluta voluptas recusandae excepturi, ducimus repudiandae? Vitae maiores suscipit eaque?</p>
        </div>
        <div class="small-container mx-5">
          <div class="testimonial-pic">
            <img src="../assets/img/avada-movers-johnsmith-final-200x200.jpg" alt="">
          </div>
          <h4>John Smith</h4>
          <p class="text-center">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptatem ut accusantium deserunt esse sapiente consequuntur aperiam architecto assumenda ullam minima soluta voluptas recusandae excepturi, ducimus repudiandae? Vitae maiores suscipit eaque?</p>
        </div>
      </div>
      <button class="btn-big">READ MORE TESTIMONIALS</button>
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
      background-color: rgba($color: $mercury, $alpha: .2);
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
          width: calc(100% / 3 - 17px);
          height: 406px;
          margin: 0 17px;
          padding: 15px;
          background-color: rgba($color: $mercury, $alpha: .4);
          border-color: $white;
        }
        .text-card{
          padding: 22px 17px;
          background-color: $white;
        }

      }
    }
    .move-with-ease{
      height: 535px;
      background-image: url(../assets/img/avada-movers-movewithease-background-new.jpg);
      @include background('');
      .container{
        display: flex;
        justify-content: end;
        .content{
          width: 415px;
          height: 295px;
          padding: 40px;
          border: 11px solid #5ca70a;
          @include flex('center');
          background-color: $lima;
          color: $white;
        }
      }
    }
    .testimonials{
      height: 670px;
      background-image: url(../assets/img/avada-movers-testimonial-background.jpg);
      @include background('');
      .container{
        @include flex('');
        .testimonial-pic{
          width: 100px;
          height: 100px;
          overflow: hidden;
          border-radius: 50%;
        }
      }
      
    }
    .request-free-quote{
      height: 370px;
      background-image: url(../assets/img/avada-movers-request-quote-background.jpg);
      @include background('');

    }
  }
</style>