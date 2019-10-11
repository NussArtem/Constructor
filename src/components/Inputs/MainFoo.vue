<template>
    <div style="background: #333333;" class=" mt-5 container-fluid">
<div class="col-lg-12 row">
        <div class="col-sm-5" style="text-align: left">
            <img src="../../../public/assets/image/logo.svg" alt="" class="mt-4 ">
            <p class="log">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                incididunt&</p>
        </div>
        <div class="col-lg-3 mt-4 " style="text-align: center">
            <p class="log1 " style="">Публичная оферта </p><p class="log1 " style="">Рекламация</p>
            <br>
            <p class="Green mt-5 ">Copyright 2019 <br>Green Soft</p>
        </div>
        <div class="col-sm-3  mt-4 ml-5">
            <span class="row">
          <img src="../../../public/assets/image/robor.svg"
               alt=""><p class="ts mt-3 ml-3">Подписаться на бота</p>   </span>
            <span class="row mt-3">
              <img src="../../../public/assets/image/facebook.svg"
                   alt=""><p class="ts  mt-3 ml-3">Поделиться на Facebook</p></span>

        </div>

    </div>
        <br><br>
    </div>
</template>

<script>
    export default {
        name: "Footer"
    }
</script>

<style scoped>
    @media screen and (max-width: 700px) {
        .container-fluid{
text-align: center        }

    }
    .container-fluid{
        display: block;
    }
        .ts {
        font-family: Helvetica Neue;
        font-size: 18px;
        line-height: 21px;
        text-align: center;
        text-decoration-line: underline;

        color: #FFFFFF;


    }


    .Green {
        font-family: Helvetica Neue;
        font-size: 18px;
        line-height: 22px;

        color: #FFFFFF;

        border-radius: 2px;


    }

    .log1 {
        font-family: Helvetica Neue;
        line-height: 29px;
        font-size: 18px;
        color: #FFFFFF;

        text-decoration-line: underline;

    }

    .log {
        font-family: Helvetica Neue;
        font-size: 18px;
        line-height: 22px;

        color: #FFFFFF;

        border-radius: 2px;

    }

</style>