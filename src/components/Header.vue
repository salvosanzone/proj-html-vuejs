<template>

  <header>
    <div class="top-header">
      <div class="container">
        <div>left</div>
        <div>right</div>
      </div>
    </div>
    <div class="bottom-header" >
      <div class="container">
        <div class="logo">logo</div>
        <div class="menu">menu</div>
      </div>
      <div class="center-container ">we make it simple</div>
    </div>
  </header>

</template>

<script>
export default {
  name: 'Header'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/mixins.scss';

header{
  .top-header{
    height: 30px;
    background-color: #69bf14;
    color: white;
    .container{
      @include flex('between');
      border: 1px solid black;
    }
  }
  .bottom-header{
    height: 535px;
    background-image: url(../assets/img/avada-movers-homeherobackground-final.jpg);
    @include background('');
    .container{
      @include flex('between')
    }
    .center-container{
    }
  }
}
  
</style>