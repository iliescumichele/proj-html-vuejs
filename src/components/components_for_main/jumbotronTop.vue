<template>
    <div class="jumbotron">

        <div class="jumbo-content">
            <div class=" ">

                <navComponent />
                


                <div class="big-text">

                </div>
            </div>
        </div>

    </div>
</template>

<script>
import navComponent from './navComponent.vue'


export default {
    name: 'jumbotronTop',
    components: {
    navComponent
  }
}

</script>

<style lang="scss" scoped>
    .jumbotron{
        height: 500px;
        background-image: url(../../assets/img/jumbo.jpg);

        .jumbo-content{
            height: 500px;
            background-color: rgba(0, 0, 0, 0.55);
        }
    }
</style>