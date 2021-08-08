<template>
    <div class="container">
        <section class="partners">
            <h2 class="partners__title">Нам доверяют</h2>
            <div class="partners__logos">
                <a href="#"><img src="../assets/p1.png" alt="" class="partners__logo"></a>
                <a href="#"><img src="../assets/p2.png" alt="" class="partners__logo"></a>
                <a href="#"><img src="../assets/p3.png" alt="" class="partners__logo"></a>
                <a href="#"><img src="../assets/p4.png" alt="" class="partners__logo"></a>
                <a href="#"><img src="../assets/p5.png" alt="" class="partners__logo"></a>
                <a href="#"><img src="../assets/p6.png" alt="" class="partners__logo"></a>
                <a href="#"><img src="../assets/p7.png" alt="" class="partners__logo"></a>
                <a href="#"><img src="../assets/p8.png" alt="" class="partners__logo"></a>
                <a href="#"><img src="../assets/p9.png" alt="" class="partners__logo"></a>
                <a href="#"><img src="../assets/p10.png" alt="" class="partners__logo"></a>
                <a href="#"><img src="../assets/p11.png" alt="" class="partners__logo"></a>
                <a href="#"><img src="../assets/p12.png" alt="" class="partners__logo"></a>
                <a href="#"><img src="../assets/p13.png" alt="" class="partners__logo"></a>
                <a href="#"><img src="../assets/p14.png" alt="" class="partners__logo"></a>
                <a href="#"><img src="../assets/p15.png" alt="" class="partners__logo"></a>
                <a href="#"><img src="../assets/p16.png" alt="" class="partners__logo"></a>

            </div>
            <p class="partners__text">и десятки других популярных компаний</p>
        </section>
    </div>
</template>

<script>
export default {
    name: "Partners",
}
</script>

<style lang="scss">
.partners {
    padding: 50px 0;
    text-align: center;
    &__title {
        font-weight: 900;
        font-size: 30px;
        line-height: 37px;
        text-transform: uppercase;
        color: #000000;
        margin-bottom: 80px;
    }
    &__text {
        font-weight: 500;
        font-size: 20px;
        line-height: 24px;
        color: #939393;
        margin-top: 50px;
    }
    &__logos {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
        gap: 50px;
        padding: 0px 50px;
    }
    &__logo {
        max-width: 250px;
        width: 100%;
    }
}
@media only screen and (max-width: 750px) {
    .partners {
        &__title {
            font-size: 20px;
            line-height: 25px;
            margin-bottom: 40px;
        }
        &__text {
            font-size: 13px;
            line-height: 15px;
        }
        &__logos {
            padding: 0;
            gap: 15px;
        }
        &__logo {
            max-width: 150px;
            width: 100%;
        }
    }
}
</style>