<template>
    <div style="display: flex;justify-content: center" class="mt-5">
        <div class="" style="
        display: flex;
        flex-direction: column;
        justify-content: center;
        justify-items: center">
            <input type="text" placeholder="Номер телефона">
            <input type="text" placeholder="ФИО">
            <input type="text" placeholder="Страна">
            <input type="text" placeholder="Город">
            <input type="text" placeholder="Почтовый индекс">
            <input type="text" placeholder="Адрес">
        </div>

    </div>
</template>

<script>
    export default {
        name: "ContactInputs"
    }
</script>


<style scoped>
    @media screen and (max-width: 700px) {

        input{
            border: none;
            margin-top: 10px;
            max-width: 323px;
            height: 60px;
            background: #FFFFFF;
            box-shadow: 0px 2px 6px rgba(0, 0, 0, 0.25);
            border-radius: 2px;
        }


    }
        input::placeholder {
        color: #CECECE;
        font-size: 18px;
        margin-left: 35px;
        padding: 0 12px;


    }
    input{
        border: none;
        margin-top: 10px;

        width: 390px;
        height: 60px;
        background: #FFFFFF;
        box-shadow: 0px 2px 6px rgba(0, 0, 0, 0.25);
        border-radius: 2px;
    }


</style>