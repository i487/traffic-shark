<template>
    <section class="forms">
        <div class="container">
            <form action="#" class="form">
                <h2 class="form__title">Остались вопросы? Готовы ответить!</h2>
                <input type="text" class="form__input" placeholder="Ваше имя">
                <input type="text" class="form__input" placeholder="Ваши контакты">
                <input type="text" class="form__input" placeholder="Ваше предложение">
                <button class="form__btn">написать нам</button>
            </form>
        </div>
    </section>
</template>

<script>
export default {
    name: "Form"
}
</script>

<style lang="scss">
.forms {
    background-image: url('../assets/mask.png');
    background-size: cover;
    background-repeat: no-repeat;
    padding-top: 400px;
    padding-bottom: 200px;

    .form {
        display: flex;
        flex-direction: column;
        gap: 42px;
        padding: 0 100px;
        &__title {
            font-weight: 900;
            font-size: 30px;
            line-height: 37px;
            text-align: center;
            color: #FFFFFF;
        }
        &__input {
            background: #FFFFFF;
            border-radius: 40px;
            font-weight: 500;
            font-size: 20px;
            line-height: 24px;
            color: rgba(126, 126, 126, 0.5);
            padding: 28px 30px;
            border: none;
            outline: none;
        }
        &__btn {
            margin: auto;
            background: transparent;
            border: 1px solid #FFFFFF;
            border-radius: 40px;
            font-weight: 900;
            font-size: 20px;
            line-height: 24px;
            text-transform: uppercase;
            color: #FFFFFF;
            padding: 20px 38px;
            cursor: pointer;
        }
    }
}
@media only screen and (max-width: 750px) {
    .forms {
        padding-top: 350px;
        .form {
            padding: 0;
            padding-bottom: 200px;
            &__title {
                font-size: 20px;
                line-height: 25px;
            }
        }
    }
}
</style>