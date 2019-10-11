<template>
    <div>

        <div class="main mt-4" >
        <span class="row mt-4">
        <p class="price">Доставка:</p>
    <span class=" value">
            <p><b>100</b>ua</p>
    </span>
        </span>

        </div>
        <div class="main mt-4" >
        <span class="row mt-4">
        <p class="price">Всего к оплате:</p>
    <span class=" value">
            <p><b>300</b>ua</p>
    </span>
        </span>

        </div>

    </div>
</template>

<script>
    export default {
        name: "FinalInput"
    }
</script>

<style scoped>
    .price{
        margin-top: 20px;
        margin-right: 10px;
        font-family: Helvetica Neue;
        font-size: 18px;
        line-height: 22px;
        /* identical to box height */

        text-align: center;

        color: #333333;
    }
    .main {
        display:flex;
        justify-content: center;
        justify-items: center;
    }

    .value {
        border: 1px solid #333333;
        box-sizing: border-box;
        border-radius: 2px;
        width: 150px;
        height: 60px;
        font-family: Helvetica Neue;
        font-size: 48px;
        line-height: 57px;
        text-align: center;

        color: #333333;


    }
</style>