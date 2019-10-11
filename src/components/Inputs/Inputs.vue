<template>
    <div>
        <div class="d-flex justify-content-center mt-5 ">

            <input type="" placeholder="Имя"><input type="text" placeholder="Фамилия">
        </div>
        <div class="d-flex justify-content-center mt-3 info">
            <input type="text" placeholder="День"><input type="text" placeholder="Месяц"><input type="text"
                                                                                                placeholder="Год">
        </div>
        <span class="mt-4 " style=" display: flex;
        justify-content: center;
        justify-items : center;">
            <button id="red"></button>
            <button id="yellow"></button>
            <button id="green"></button>
            <button id="blue"></button>
            <button id="black"></button>
        </span>
        <span class="mt-4 size" style=" display: flex;
        justify-content: center;
        justify-items : center;">
            <button>XS</button>
            <button>S</button>
            <button>M</button>
            <button>L</button>
            <button>XL</button>
            <button>XXL</button>

        </span>
        <price></price>
        <div class="mt-4 btnGet" style="display: flex;justify-items: center;justify-content: center">
            <button>Добавить</button>
        </div>
        <p class="mt-4"> Данные для доставки</p>
        <contact-inputs class="mt-4"></contact-inputs>
        <p class="mt-4 Backet">Корзина</p>

        <basket></basket>
        <final-input class="mt-2"></final-input>
        <div class="mt-5 btnGet" style="display: flex;justify-items: center;justify-content: center">
            <button>Оплатить</button>
        </div>
        <main-foo></main-foo>
    </div>
</template>

<script>
    import MainFoo from "@/components/Inputs/MainFoo";
    import FinalInput from "@/components/Inputs/FinalInput";
    import Basket from "@/components/Inputs/Basket";
    import ContactInputs from "@/components/Inputs/ContactInputs";
    import Price from "@/components/Inputs/Price";

    export default {
        name: "Inputs",
        components: {Price, ContactInputs, Basket, FinalInput, MainFoo}
    }
</script>

<style scoped>
    @media screen and (max-width: 700px) {
        .btnGet button {
            max-width: 250px;
            max-height: 40px;
            background: #333333;
            border-radius: 30px;
            font-family: Helvetica Neue;
            font-size: 18px;
            line-height: 21px;
            text-align: center;
            color: #FDFDFD;
        }

        .info input{
            border: none;
            width: 100px;

        }
    }

    .Backet {
        font-family: Helvetica Neue;
        font-size: 24px;
        line-height: 29px;
        /* identical to box height */
        text-align: center;
        color: #333333;

    }

    .btnGet button {
        border: none;

        width: 390px;
        height: 60px;
        background: #333333;
        border-radius: 30px;
        font-family: Helvetica Neue;
        font-size: 18px;
        line-height: 21px;
        text-align: center;
        color: #FDFDFD;
    }

    .size button {
        width: 40px;
        height: 40px;
        background: #FFFFFF;
        box-shadow: 0px 2px 6px rgba(0, 0, 0, 0.25);
        border-radius: 2px;
        font-family: Helvetica Neue;
        font-size: 15px;
        line-height: 21px;
        text-align: center;
        color: #333333;
        margin-right: 13px;

    }

    input {
        font-family: Helvetica Neue;
        min-width: 100px;
        max-width: 152px;
        height: 44px;
        background: #FFFFFF;
        box-shadow: 0px 2px 6px rgba(0, 0, 0, 0.25);
        border-radius: 2px;
        border: none;
        padding: 0 12px;
        margin-right: 15px;
    }

    input::placeholder {
        color: #CECECE;
        font-size: 18px;
        margin-left: 25px;


    }

    #red {


        width: 35px;
        height: 35px;
        background: red;
        box-shadow: 0px 2px 6px rgba(0, 0, 0, 0.25);
        border: none;

        border: none;
        border-radius: 50%;
        margin-right: 10px;

    }

    #yellow {


        width: 35px;
        height: 35px;
        background: #FFF730;
        box-shadow: 0px 2px 6px rgba(0, 0, 0, 0.25);
        border: none;
        border-radius: 50%;
        margin-right: 10px;

    }

    #green {


        width: 35px;
        height: 35px;
        background: #63E768;
        box-shadow: 0px 2px 6px rgba(0, 0, 0, 0.25);
        border: none;
        border-radius: 50%;
        margin-right: 10px;

    }

    #blue {


        width: 35px;
        height: 35px;
        background: #4C6BDB;
        box-shadow: 0px 2px 6px rgba(0, 0, 0, 0.25);
        border: none;
        border-radius: 50%;
        margin-right: 10px;

    }

    p {
        font-family: Helvetica Neue;
        font-size: 34px;
        line-height: 42px;
        /* identical to box height */

        text-align: center;

        color: #333333;


    }

    #black {


        width: 35px;
        height: 35px;
        background: #000000;
        box-shadow: 0px 2px 6px rgba(0, 0, 0, 0.25);
        border: none;
        border-radius: 50%;
        margin-right: 10px;

    }
</style>