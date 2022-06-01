<template>
    <div class="percentage-text my-5">
        <div class="percentage">
            <div class="single-chart">
                <svg viewBox="0 0 36 36" class="circular-chart green">
                    <path class="circle-bg"
                    d="M18 2.0845 a 15.9155 15.9155 0 0 1 0 31.831 a 15.9155 15.9155 0 0 1 0 -31.831"/>
                    <path class="circle" :stroke-dasharray="`${cardData.percentage}, 100`" d="M18 2.0845 a 15.9155 15.9155 0 0 1 0 31.831 a 15.9155 15.9155 0 0 1 0 -31.831"/>
                <text x="18" y="20.35" class="percentage">{{cardData.percentage}}%</text>
                </svg>
            </div>
        </div>
        <div class="text">
            <p class="title-percentage">{{cardData.title}}</p>
            <p class="descr-percentage">{{cardData.description}}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'cardPercentages',
    props: { cardData: Object }
}
</script>

<style lang="scss" scoped>
@import '../../../assets/style/vars';

.percentage-text{
        display: flex;
        justify-content: space-between;
        align-items: center;

        .text{
            margin-left: 50px;
        }

        .title-percentage{
            font-size: 2.5rem;
            font-weight: 800;
            color: white;
        }

        .descr-percentage{
            color: $colorCube_manatee;
        }

        .single-chart {
            text{
                font-size: 2rem;
                font-weight: 800;
            }

            .circular-chart {
              display: block;
              margin: 10px auto;
              width: 100px;
            }
            .circle-bg {
              fill: none;
              stroke: rgba(238, 238, 238, 0.24);
              stroke-width: 4;
            }
            .circle {
              fill: none;
              stroke-width: 4;
              stroke-linecap: round;
              animation: progress 1s ease-out forwards;
            }
            @keyframes progress {
              0% {
                stroke-dasharray: 0 100;
              }
            }
            .circular-chart.green .circle {
              stroke: $materialDesign_elfGreen;
            }
            .percentage {
              fill: #8d959f;
              font-family: sans-serif;
              font-size: 0.5em;
              text-anchor: middle;
            }
        }
    }

</style>