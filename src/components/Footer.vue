<template>

  <footer>
    <!-- TOP FOOTER -->
    <div class="top-footer">
      <div class="big-container">
        <div
          class="small-container align-items-start me-5 justify-content-around"
        >
          <span class="">ABOUT</span>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod amet
            repellat vero placeat fugit et commodi nulla exercitationem
            excepturi, officiis ullam explicabo quo voluptas, accusantium quos
            illum veritatis harum in.
          </p>
          <div class="logo-footer">
            <img src="../assets/img/avada-movers-retinalogo.png" alt="" />
          </div>
        </div>
        <div class="small-container align-items-start justify-content-around">
          <span>AVADA MOVERS</span>
          <span v-for="item in avadaMovers" :key="item.id">
            <i class="fas fa-chevron-right active"></i>
            <a
              :class="{ active: item.actived === true }"
              @click="item.actived = !item.active"
              :href="item.name"
            >
              {{ item.name }}
            </a>
          </span>
        </div>
        <div class="small-container align-items-start justify-content-around">
          <span>RECENT POSTS</span>
          <span v-for="(item, index) in recentPosts" :key="index">
            <i class="fas fa-chevron-right"></i>
            <a :href="item.name">
              {{ item.name }}
            </a>
          </span>
        </div>
      </div>
    </div>
    <!-- /TOP FOOTER -->

    <!-- BOTTOM FOOTER -->
    <div class="bottom-footer">
      <div class="small-container">
        <i class="far fa-copyright my-3">
          Copyright 2012 - 2020 | Avada Theme by ThemeFusion | All Rights
          Reserved | Powered by WordPress</i
        >
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
      <div class="get-back-arrow">
        <a href="">
          <i class="fas fa-chevron-up"></i>
        </a>
      </div>
    </div>
    <!-- /BOTTOM FOOTER -->
  </footer>

</template>

<script>
export default {
  name: "Footer",

  props: {
    //Footer riceve da App due array tramite le props
    avadaMovers: Array,
    recentPosts: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";
@import "../assets/style/mixins.scss";

footer {
  .top-footer {
    @include flex("center");
    height: 300px;
    border-top: 10px solid $lima;
    .big-container {
      @include flex("");
      .logo-footer {
        width: 120px;
      }
      .small-container {
        span {
          font-weight: 800;
          font-size: 12px;
          margin-bottom: 15px;
          i {
            color: $river-bed;
            margin-right: 2px;
          }
          a {
            font-weight: normal;
          }
        }
        p {
          font-weight: 700;
          color: $river-bed;
        }
      }

      i,
      a {
        color: $black;
        &:hover {
          color: $mantis;
        }
      }
      a.active {
        color: $mantis !important;
      }
    }
  }
  .bottom-footer {
    position: relative;
    @include flex("center");
    height: 95px;
    background-color: $lima;
    .small-container {
      a {
        font-size: 13px;
      }
    }
  }
  .get-back-arrow {
    position: absolute;
    bottom: 0;
    right: 50px;
    width: 32px;
    height: 20px;
    @include flex("center");
    background-color: $river-bed;
    border-radius: 2px;
    i {
      color: $mercury;
    }
  }
}
</style>