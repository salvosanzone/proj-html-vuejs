<template>

  <footer>
    <div class="top-footer">
      <div class="container">
        top footer
      </div>
    </div>
    <div class="bottom-footer">
      <div class="center-container">
        bottom footer
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
      height: 300px;
      border-top: 10px solid $lima;
    }
    .bottom-footer{
      height: 95px;
      background-color: $lima;
    }
  }

</style>