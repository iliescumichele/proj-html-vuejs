<template>
  <section id="latest-news">
    <div class="container">
        <div class="text-news">
            <h4>OUR EDITORIAL CONTENT</h4>
            <h2 class="my-4">Latest <span>News</span></h2>
            <div class="litle-text-and-button-underlatest-news-title mt-4">
                <p class="">Every week we publish content about what is best in the business world.</p>
                <button type="button" class="btn">SEE ALL</button> 
            </div>

            <div class="cards container-fluid mt-3">
                <div class="row row-cols-3 ">
                   
                    <cardLatestNews
                        v-for="(cardItem, index) in cardLatestNewsList"
                        :key="`cardItem${index}`"
                        :cardData="cardItem"
                    />

                </div>
            </div>
        </div>
    </div>
  </section>
</template>

<script>
import cardLatestNews from "./cards/cardLatestNews.vue"

export default {
    name: 'latestNewsSectionComponent',
    components: { cardLatestNews },
    data(){
        return{
            cardLatestNewsList: [
                {
                    "thumb": "news-1.jpg",
                    "text": "Increasing creativity is possible for everyone"
                },
                {
                    "thumb": "news-2.jpg",
                    "text": "Because market research is part of our busoness plan"
                },
                {
                    "thumb": "news-3.jpg",
                    "text": "Working from home is now a trend"
                },
                {
                    "thumb": "news-4.jpg",
                    "text": "Working in the office has its benefits"
                },
                {
                    "thumb": "news-5.jpg",
                    "text": "Increasing creativity is possible for everyone"
                },
            ]
        }
    }
};
</script>

<style lang="scss" scoped>
@import '../../assets/style/vars';

    section{
        padding-bottom: 120px;
        background-color: #ffffff;
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

    .text-news{
        padding-top: 100px;

        h4{ 
            font-size: 0.9rem;
            font-weight: 800;
            color: $materialDesign_elfGreen;
        }
        
        h2{
            font-size: 3rem;
            font-weight: 800;

            span{ 
                color: $materialDesign_elfGreen;
                background-color: $materialDesign_elfGreenAlpha;
            }
        }

        p{
            font-size: 1.15rem;
            color: $colorCube_manatee;
        }

        .litle-text-and-button-underlatest-news-title{ 
            display: flex;
            justify-content: space-between;
            align-items: center;

            .btn{ 
                background-color: $colorCube_blueLagoon;
                color: $medinCut_grayNurse;
                padding: 9px 20px;
            }
        }
    }
</style>