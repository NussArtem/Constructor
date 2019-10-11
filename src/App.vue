<template>
    <div class="app-container">

        <header-main></header-main>
        <slider-content></slider-content>

    </div>
</template>

<script>
    import HeaderMain from "@/components/HeaderMain/HeaderMain";
    import SliderContent from "@/components/SliderContent/SliderContent";

    export default {
        name: 'app',
        components: {
            HeaderMain, SliderContent,

        }
    }
</script>

<style>
    #app {
        margin-left: auto;
        margin-right: auto;
        background: #E5E5E5;
        font-family: Helvetica Neue;
        min-height: 100vh;


    }
</style>
