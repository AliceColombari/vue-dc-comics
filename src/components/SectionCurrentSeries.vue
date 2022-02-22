<template>
  <div class="card">
      <img class="card-image" :src="image" alt="">
      <h6 class="card-title">{{title.toUpperCase()}}</h6>
  </div>
</template>

<script>
export default {
    name: 'SectionCurrentSeries',
    props: {
        image: String,
        title: String
    }
}
</script>

<style scoped lang="scss">

@import "../assets/style/variabili.scss";

    .card {
       width: calc(100% / 6);
       margin-top: 30px;
       padding: 0px 5px;

       &:hover {
               cursor: pointer;
        }


       .card-image {
           width: 160px;
           height: 160px;
           object-fit: cover;
           object-position: top;

       }

       .card-title {
           margin-top: 12px;
           color: $light;
           font-size: 12px;
       }
    }
</style>