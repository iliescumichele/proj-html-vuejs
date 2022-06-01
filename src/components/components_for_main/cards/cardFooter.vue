<template>
  <div class="col">
    <div class="card p-4">
      <p class="top-title-card">{{cardData.title}}</p>
      <ul>
        <li v-for="(item) in cardData.links" :key="item"><i class="fa-solid fa-chevron-right"></i><a href="#">{{item}}</a></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
    name: 'cardFooter',
    props: { cardData: Object }
}
</script>

<style lang="scss" scoped>
@import '../../../assets/style/vars.scss';

    .card{
        background-color: $colorCube_saltpanAlpha;
        border-radius: 15px;
        color: white;

        p{
          font-size: 1.4rem;
          font-weight: bold;
        }

        li:hover{
          text-decoration: underline;
        }

        li{
          margin: 10px 0;
          list-style: none;
          a{  
            margin-left: 10px;
            text-decoration: none;
            color: $colorCube_saltpan;
          }
        }
    }
</style>