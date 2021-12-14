<template>
  <div class="card">
          <div class="pic-card d-flex justify-content-center">
            <img 
              :src="require(`../assets/img/avada-movers-${cardData.photo}`)" :alt="cardData.title"
            >
          </div>
          <div class="text-card text-center">
            <h5>{{cardData.title}}</h5>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas debitis aspernatur odio suscipit asperiores eaque unde, minus repellendus eveniet repellat dicta perferendis? Eaque architecto doloremque incidunt assumenda vel necessitatibus ipsam.</p>
            <button class="btn-small">READ MORE</button>
          </div>
        </div>
</template>

<script>
export default {
  name: 'Cards',
  props:{
    cardData: Object
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";

.card{
  display: flex;
  justify-content: space-between;
  width: calc(100% / 3 - 17px);
  height: 415px;
  margin: 0 17px;
  padding: 15px;
  background-color: rgba($color: $mercury, $alpha: .4);
  border-color: $white;
}
.text-card{
  padding: 15px 17px;
  background-color: $white;
  h5{
    color: $denim-vibrant;
    font-weight: 700;
  }
  p{
    color: $oslo-gray;
    font-weight: 800;
  }
}

</style>