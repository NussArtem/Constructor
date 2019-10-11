<template>
    <div class="mt-4">
        <flickity ref="flickity" :options="flickityOptions">
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>

        </flickity>
        <div class="small">
            <small-slider></small-slider>
        </div>
        <inputs></inputs>

    </div>
</template>

<script>
    import Flickity from 'vue-flickity';
    import SmallSlider from "@/components/SliderContent/SmallSlider";
    import Inputs from "@/components/Inputs/Inputs";

    export default {
        name: "SliderContent",
        components: {
            Flickity, SmallSlider,Inputs
        },

        data() {
            return {
                flickityOptions: {
                    groupCells: true,
                    initialIndex: 0,
                    prevNextButtons: false,
                    pageDots: false,
                    wrapAround: true

                    // any options from Flickity can be used
                }
            }
        },


    }
</script>

<style scoped>
    .small {
        display: block;
        position: relative;
        left: 20%;
        width:60%;
    }

    /* external css: flickity.css */

    * {
        box-sizing: border-box;
    }


    .carousel {
        background: #FAFAFA;
    }

    .carousel-cell {
        width: 650px;
        height: 480px;
        background-image: url("../../../public/assets/image/slide.svg");
        border-radius: 2px;
        border: 1px solid #333333;
        counter-increment: carousel-cell;
        margin-right: 15px;
    }

    /* cell number */
    .carousel-cell:before {
        display: block;
        text-align: center;
        content: counter(carousel-cell);
        line-height: 200px;
        font-size: 80px;
        color: white;
    }

</style>