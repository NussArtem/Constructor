<template>
    <div class="mt-5">
        <flickity ref="flickity" :options="flickityOptions">
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>  <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
        </flickity>
    </div>
</template>

<script>
    import Flickity from 'vue-flickity';

    export default {
        name: "SliderContent",
        components: {
            Flickity
        },

        data() {
            return {
                flickityOptions: {
                    groupCells: 1,
                    initialIndex: 4,
                    pageDots: false,
                    wrapAround: true,
                    prevNextButtons: false,


                    // any options from Flickity can be used
                }
            }
        },


    }
</script>

<style scoped>

    /* external css: flickity.css */

    * {
        box-sizing: border-box;
    }

    body {
        font-family: sans-serif;
    }


    .carousel-cell {

        width: 78px;
        height: 74px;
        background-image: url("../../../public/assets/image/smallT.svg");
        border-radius: 2px;
        border: 1px solid #333333;
        counter-increment: carousel-cell;
        margin-right: 20px;

    }

    /* cell number */
    .carousel-cell:before {
        display: block;
        text-align: center;
        content: counter(carousel-cell);
        line-height: 200px;
        font-size: 80px;
    }

</style>