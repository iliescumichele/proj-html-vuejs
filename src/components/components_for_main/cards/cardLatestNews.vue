<template>
  <div class="col py-3">
    <div class="my-card">
      <div class="card-text">
        <p>{{cardData.text}}</p>
      </div>
      <img :src="getImgUrl(cardData.thumb)" alt="">
    </div>
  </div>
</template>

<script>
export default {
  name : 'cardLatestNews',
  props: { cardData: Object },

  methods:{
    getImgUrl(thumb){
      return require('../../../assets/img/' + thumb)
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../../../assets/style/vars';
  .my-card:hover{
    cursor: pointer;

    .card-text{ 
      background-color: rgba(0, 0, 0, 0.2);
    }

    p{ 
      text-shadow: 3px 3px black;
    }
  }

  .my-card{
    width: 98%;
    position: relative;
    border-radius: 15px;
    overflow: hidden;

    img{
      width: 100%;
    }

    .card-text{
      width: 100%;
      height: 100%;
      position: absolute;
      text-align: center;
      padding: 20px 15px;
      background-color: rgba(0, 0, 0, 0.4);
      display: flex;
      align-items: flex-end;
        
      p{
          color: $colorCube_saltpan;
          font-weight: bold;
          font-size: 1.4rem;
          line-height: 25px;
      }
    }
  }
</style>