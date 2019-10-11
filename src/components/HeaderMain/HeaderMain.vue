<template>
    <div class="mainContainer col-12 row" style="display: flex;justify-content: space-between">

        <img src="../../../public/assets/image/logo.svg" class="ml-5 col-2 logo" width="200" height="52">
        <span class="row col-5 ml-3">
        <p class="lang mt-4 ">Язык:</p>
        <div class="dropdown d-inline-block ">
            <img src="../../../public/assets/image/uk.svg" alt="" class="dropbtn mt-1" style="position: relative;left: 10px">
            <div class="dropdown-content">
                <a href="#" ><img src="../../../public/assets/image/poland.svg" alt="">Poland</a>
                <a href="#"><img src="../../../public/assets/image/uk_s.svg" alt="">Ukraine</a>
                <a href="#"><img src="../../../public/assets/image/rus.svg" alt="">Russia</a>
                <a href="#"><img src="../../../public/assets/image/usa.svg" alt="">USA</a>
            </div>
        </div>
    </span>
        <span class="row land mr-2" >

             <p class="lang mt-4" >Сегодня:   </p><a class="Numb mt-1 mr-2">1233</a>

         <img src="../../../public/assets/image/uk.svg" alt="" class="mb-3">


        </span>


    </div>

</template>

<script>
    export default {
        name: "HeaderMain"
    }
</script>

<style scoped>
    @media (max-width: 700px) {
        .land{
            display: none;
        }
        .logo{
            min-width: 140px;
            min-height: 32px;
            margin-top: 10px;
        }
    }
    .Numb {
        font-family: Helvetica Neue;
        font-size: 48px;
        line-height: 57px;
        text-align: center;
        color: #FFFFFF;
    }
    .dropbtn {

        border: none;
    }
    .dropdown {
        display: inline-block;
    }

    .dropdown-content {
        display: none;
        position: absolute;
        background: #EEEEEE;
        min-width: 120px;
        border-radius: 2px;
        box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
        z-index: 1;
    }

    .dropdown-content a {
        font-family: Roboto;
        font-style: normal;
        font-weight: 300;
        font-size: 14px;
        line-height: 16px;
        color: #333333;
        padding: 12px 12px;
        text-decoration: none;
        display: flex;
        justify-content: space-between;
        justify-items: center;
    }

    .dropdown-content a:hover {
        background: #CECECE;
        box-shadow: 0px 2px 6px rgba(0, 0, 0, 0.25);


    }

    .dropdown:hover .dropdown-content {
        display: block;
    }

    .dropdown:hover .dropbtn {
        box-shadow: 0px 2px 6px rgba(0, 0, 0, 0.25);
        border-radius: 2px;
    }

    .lang {
        font-size: 18px;
        line-height: 21px;
        text-align: center;
        color: #FFFFFF;
    }

    .mainContainer2 {

    }

    .mainContainer {
        font-family: Helvetica Neue;
        justify-items: center;
        height: 80px;
        width: 100vw;
        background-color: #333333;
        font-size: 18px;
        line-height: 21px;
        text-align: center;
        color: #FFFFFF;
        margin-left: 0;
    }


</style>