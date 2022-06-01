<template>
    <div class="col">
        <div class="my-card p-5 h-100">
            <img class="w-100" :src="getImgUrl(cardData.thumb)" alt="">
            <div class="text ">
                <h3 class="my-4">{{cardData.title}}</h3>
                <p>{{cardData.description}}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'cardLogistics',
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

    .col{ 
        width: 30%;
        margin: auto 10px;

        .my-card{ 
            border-radius: 15px;
            background-color: white;

            h3{ 
                font-weight: 600;
            }

            p{ 
                font-size: 1.15rem;
            }
        }
        
    }
</style>