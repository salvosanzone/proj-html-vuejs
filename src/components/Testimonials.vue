<template>
  <div class="small-container mx-5">
    <div class="testimonial-pic">
      <img 
        :src="require(`../assets/img/avada-movers-${testimonialData.photo}`)" :alt="testimonialData.name"
      >
    </div>
    <h5>{{testimonialData.name}}</h5>
    <p class="text-center">"Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptatem ut accusantium deserunt esse sapiente consequuntur."</p>
  </div>
</template>

<script>
export default {
  name: 'Testimonials',
  props:{
    testimonialData: Object
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";
  .testimonial-pic{
    width: 100px;
    height: 100px;
    overflow: hidden;
    border-radius: 50%;
  }
  .small-container{
    h5{
      color: $denim-vibrant;
      font-weight: 700;
      margin: 15px 0;
    }
  }
</style>