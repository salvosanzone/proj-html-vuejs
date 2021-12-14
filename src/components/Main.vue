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
        <p class="text-center">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta in illo earum aspernatur pariatur ea iste nihil officia ipsam veritatis. Necessitatibus non temporibus iure fugiat officiis rem inventore natus iste.</p>
        <button class="btn-big">REAR OUR TESTIMONIALS</button>
      </div>
    </section>
    <section class="full-service">
      <div class="small-container">
        <span>WE ARE A PROFESSIONAL</span>
        <h2>Full-Service Solution</h2>
      </div>
      <div class="big-container">
        <Card 
          v-for="card in cardList" 
          :key="card.id"
          :cardData="card"
        />
      </div>
    </section>
    <section class="move-with-ease">
      <div class="big-container">
        <div class="content flex-column">
          <span>WE REMOVE THE HEADACHE FROM MOVING</span>
          <h2>Move with Ease</h2>
          <p class="text-center">With our super simple service we can take you from getting a quote, right throught to being in your new home with all of your belongings securely packed and safely delivered, even in the rooms of your choice.</p>
          <button class="btn-big">GET A FREE QUOTE NOW</button>
        </div>
      </div>
    </section>
    <section class="testimonials">
      <div class="small-container">
        <span>HAPPY CUSTOMERS</span>
        <h2>Testimonials</h2>
      </div>
      <div class="big-container my-5">
        <Testimonials 
          v-for="(testimonial, index) in testimonialsList"
          :key="index"
          :testimonialData="testimonial"
        />
      </div>
      <button class="btn-big">READ MORE TESTIMONIALS</button>
    </section>
    <section class="request-free-quote">
      <div class="small-container">
        <h2>Request A Free Quote</h2>
        <p class="text-center my-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt tenetur architecto quaerat consectetur accusamus amet minima consequatur perspiciatis! Alias at asperiores nisi.</p>
        <button class="btn-small">CLICK HERE</button>
      </div>
    </section>
  </main>

</template>

<script>
import Card from './Cards.vue'
import Testimonials from './Testimonials.vue'
export default {
  name: 'Main',
  components:{
    Card,
    Testimonials
  },
  data(){
    return{
      cardList: [
        {
          photo: "serviceonephoto-final-400x255.jpg",
          title: 'Two Man Teams',
          id: 1
        },
        {
          photo: "servicetwophoto-final-400x255.jpg",
          title: 'We Do All The Lifting',
          id: 2
        },
        {
          photo: "servicethreephoto-final-400x255.jpg",
          title: 'Coast To Coast',
          id: 3
        },
      ],

      testimonialsList: [
        {
          photo: "johndoe-final-200x200.jpg",
          name: 'John Doe'
        },
        {
          photo: "janedoe-final-200x200.jpg",
          name: 'Jane Doe'
        },
        {
          photo: "johnsmith-final-200x200.jpg",
          name: 'John Smith'
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";
@import '../assets/style/mixins.scss';

  main{
    .get-free-quote{
      height: 100px;
      background-color: $denim-vibrant;
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
      span,
      p{
        color: $oslo-gray;
        font-weight: 800;
      }
      h2{
        font-weight: 700;
        color: $lima-darkVibrant;
      }
      
    }
    .full-service{
      height: 670px;
      .small-container{
        span{
          font-weight: 800; 
          color: $oslo-gray;
        }
        h2{
          font-weight: 700;
          color: $lima-darkVibrant;
          margin-bottom: 35px
        }
      }
      .big-container{
        @include flex('');
      }
    }
    .move-with-ease{
      height: 535px;
      background-image: url(../assets/img/avada-movers-movewithease-background-new.jpg);
      @include background('');
      .big-container{
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
          span{
            font-weight: 800;
          }
          h2{
            font-weight: 700;
            margin: 5px 0;
            position: relative;
            }
            h2::after{
              content: " ";
              border-bottom: 1px solid $mantis;
              display:table-cell;
              width:240px;
              position: absolute;
              top: 50px;
            }
            p{
              margin: 20px 0;
            }
        }
      }
    }
    .testimonials{
      height: 670px;
      background-image: url(../assets/img/avada-movers-testimonial-background.jpg);
      @include background('');
      .small-container{
        span{
          font-weight: 800;
          color: $oslo-gray;
        }
        h2{
          font-weight: 700;
          color: $lima-darkVibrant;
        }
        p{
          color: $oslo-gray;
          font-weight: 700;
          font-size: 11px
        }
      }
      .big-container{
        @include flex('');
      }
      
    }
    .request-free-quote{
      height: 370px;
      background-image: url(../assets/img/avada-movers-request-quote-background.jpg);
      @include background('');
      background-size: cover;
      .small-container{
        h2{
          color: $lima-darkVibrant;
          font-weight: 700;
        }
        p{
          color: $river-bed;
          font-weight: 700;
        }
      }

    }
  }
</style>