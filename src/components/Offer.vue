<template>
    <section class="offer">
        <div class="container offer__container">
            <h2 class="offer__title">мы всегда в топе!</h2>
            <p class="offer__text">Мы прямой рекламодатель с собственными офферами, которые входят в топ-чарты AppStore и Google Play. </p>

            <div class="offer__items">
                <div class="offer__item">
                    <h2 class="offer__item-title">ТОП</h2>
                    <p class="offer__item-text">Наши офферы входят в ТОПы в AppStore и Google Play</p>
                </div>
                <div class="offer__item">
                    <h2 class="offer__item-title">ОФФЕРЫ</h2>
                    <p class="offer__item-text">Мы делаем собственные белые мобильные офферы, которые вы не найдете ни в одной другой партнерке</p>
                </div>
                <div class="offer__item">
                    <h2 class="offer__item-title">2.5$</h2>
                    <p class="offer__item-text">Мы платим до $2.5 за инсталл и принимаем трафик со всего мира</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Offer"
}
</script>

<style lang="scss">
.offer {
    background-image: url('../assets/top.png');
    background-size: cover;
    background-repeat: no-repeat;
    margin-top: 100px;
    padding: 200px 0;
    &__container {
        text-align: center;
    }
    &__title {
        font-weight: 900;
        font-size: 30px;
        line-height: 37px;
        text-transform: uppercase;
        color: #FFFFFF;
        margin-bottom: 20px;
    }
    &__text {
        font-weight: 500;
        font-size: 20px;
        line-height: 24px;
        color: #FFFFFF;
        width: 55%;
        margin: auto;
        margin-bottom: 80px;
    }
    &__items {
        display: flex;
        gap: 60px;
    }
    &__item {
        flex-basis: 30%;
        &-title {
            font-size: 56px;
            line-height: 64px;
            color: white;
            margin-bottom: 12px;
        }
        &-text {
            font-weight: bold;
            font-size: 16px;
            line-height: 19px;
            color: #FFFFFF;
        }
    }
}
@media only screen and (max-width: 750px) {
    .offer {
        &__title {
            font-size: 20px;
            line-height: 25px;
        }
        &__text {
            font-size: 16px;
            line-height: 19px;
            width: auto;
        }
        &__items {
            flex-direction: column;
        }
        &__item {
            &-title {
                font-size: 46px;
                line-height: 50px;
            }
            &-text {
                font-size: 13px;
                line-height: 16px;
            }
        }
    }
}
</style>