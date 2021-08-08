<template>
    <section class="payment">
        <div class="container payment__container">
            <h2 class="payment__title">Еженедельные выплаты <span>от $100</span></h2>
            <p class="payment__text">На удобную для вас платежную систему из перечисленных ниже</p>

            <div class="payment__methods">
                <a href="#" class="link"><img src="../assets/z1.png" alt="" class="payment__methods-item"></a>
                <a href="#" class="link"><img src="../assets/z3 (1).png" alt="" class="payment__methods-item"></a>
                <a href="#" class="link"><img src="../assets/z3.png" alt="" class="payment__methods-item"></a>
                <a href="#" class="link"><img src="../assets/z4 1.png" alt="" class="payment__methods-item"></a>
                <a href="#" class="link"><img src="../assets/z5.png" alt="" class="payment__methods-item"></a>
                <a href="#" class="link"><img src="../assets/z6.png" alt="" class="payment__methods-item"></a>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Payment"
}
</script>

<style lang="scss">
.payment {
    padding: 50px 0;
    &__container {
        text-align: center;
    }
    &__title {
        font-weight: 900;
        font-size: 30px;
        line-height: 37px;
        text-transform: uppercase;
        color: #000000;
        margin-bottom: 20px;
    }
    &__text {
        font-weight: 500;
        font-size: 20px;
        line-height: 24px;
        color: #939393;
        margin-bottom: 80px;
    }
    &__methods {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 30px;
    }
}
@media only screen and (max-width: 750px) {
    .payment {
        &__title {
            font-size: 20px;
            line-height: 25px;
        }
        &__text {
            font-size: 13px;
            line-height: 17px;
        }
        &__methods {
            flex-wrap: wrap;
            gap: 18px;
        }
    }
}
</style>