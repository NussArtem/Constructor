<template>
    <div class="d-flex justify-content-sm-center">

<span class=" mt-5 main">
<label class=" container">
      <input type="checkbox" checked="checked" name="remember"> <img src="../../../public/assets/image/smallT.svg"
                                                                     alt=""><p class="ts mt-4">Футболка</p><button>XL</button>
            <span class="checkmark"></span>

        </label>
</span>
    </div>
</template>

<script>
    export default {
        name: "Basket"
    }
</script>

<style scoped>
    @media screen and (max-width: 700px) {
        .main {

        }
    }

    img {
        border: 1px solid #333333;
        box-sizing: border-box;
        border-radius: 2px;
        margin-left: 25px;
    }

    button {
        margin-top: 15px;
        margin-left: 100px;
        width: 40px;
        height: 40px;
        background: #FFFFFF;
        box-shadow: 0px 2px 6px rgba(0, 0, 0, 0.25);
        border-radius: 2px;
        font-family: Helvetica Neue;
        font-size: 18px;
        line-height: 21px;
        text-align: center;

        color: #333333;
    }

    .ts {
        font-family: Helvetica Neue;
        font-size: 18px;
        line-height: 21px;
        text-align: center;
        margin-left: 10px;
        color: #333333;
    }

    .main {
        display: inline-flex;
        justify-content: center;
        justify-items: center;
    }

    .container {
        display: flex;
        justify-content: center;
        justify-items: center;
        position: relative;
        margin-bottom: 12px;
        cursor: pointer;
        font-size: 9px;
        -webkit-user-select: none;
        -moz-user-select: none;
        -ms-user-select: none;
        user-select: none;
    }

    /* Hide the browser's default checkbox */
    .container input {
        position: absolute;
        opacity: 0;
        cursor: pointer;
        height: 0;
        width: 0;
    }

    /* Create a custom checkbox */
    .checkmark {
        position: absolute;
        top: 25px;
        left: 0;
        width: 24px;
        height: 24px;
        background: #FFFFFF;
        box-shadow: 0px 2px 6px rgba(0, 0, 0, 0.25);
        border-radius: 2px;
        border-radius: 5px;
    }

    /* On mouse-over, add a grey background color */
    .container:hover input ~ .checkmark {
        background-color: #ccc;
    }

    /* When the checkbox is checked, add a blue background */
    .container input:checked ~ .checkmark {
        background-color: #ffffff;
    }

    /* Create the checkmark/indicator (hidden when not checked) */
    .checkmark:after {
        content: "";
        position: absolute;
        display: none;
    }

    /* Show the checkmark when checked */
    .container input:checked ~ .checkmark:after {
        display: block;
    }

    .container .checkmark:after {
        right: 5px;
        bottom: 6px;
        width: 13px;
        height: 18px;
        border: solid #000000;
        border-width: 0px 2px 2px 0px;

        transform: rotate(45deg);
    }

</style>