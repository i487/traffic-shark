<template>
    <section class="coworking">
        <div class="container">
            <h2 class="title">Работать с нами это</h2>
            <div class="coworking__items">
                <div class="coworking__item" v-for="(item, index) in coworking" :key="index">
                    <span class="coworking__item-icon" v-html="item.icon">
                        <!-- <svg width="65" height="65" viewBox="0 0 65 65" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M58.3564 10.5252L33.4736 0.194095C32.8503 -0.064635 32.1496 -0.064762 31.5264 0.194095L6.64358 10.5252C5.69588 10.9187 5.07812 11.8439 5.07812 12.8701V25.4289C5.07812 42.7216 15.53 58.2768 31.5405 64.8117C32.1554 65.0627 32.8444 65.0627 33.4595 64.8117C49.4697 58.2769 59.9219 42.7217 59.9219 25.4289V12.8701C59.9219 11.8439 59.3042 10.9187 58.3564 10.5252ZM54.8438 25.4289C54.8438 40.1295 46.2109 53.6623 32.5 59.703C19.1554 53.8237 10.1562 40.5279 10.1562 25.4289V14.5652L32.5 5.28822L54.8438 14.5652V25.4289ZM29.6936 33.9874L40.607 23.0741C41.5985 22.0826 43.2061 22.0825 44.1977 23.0741C45.1893 24.0657 45.1892 25.6733 44.1976 26.6648L31.4889 39.3735C30.4972 40.3652 28.8896 40.3649 27.8982 39.3735L20.8023 32.2776C19.8107 31.2859 19.8107 29.6783 20.8023 28.6868C21.7939 27.6953 23.4015 27.6952 24.393 28.6868L29.6936 33.9874Z" fill="#2E9ADB"/>
                        </svg> -->
                    </span>
                    <p class="coworking__item-text"> {{ item.text }} </p>
                </div>
            </div>
            <button class="coworking__btn">Регистрация</button>
        </div>
    </section>
</template>
<script>
export default {
    name: "CoWorking",
    props: ["coworking"]
}
</script>

<style lang="scss">
.coworking {
    text-align: center;
    padding-top: 80px;

    &__items {
        margin-top: 60px;
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-gap: 50px 30px;
        padding: 80px 0;
    }
    &__item {
        text-align: center;
        &-icon {
            margin-bottom: 30px;
        }
        &-text {
            margin-top: 30px;
            font-weight: 300;
            font-size: 20px;
            line-height: 23px;
            color: #000000;
            padding: 0 20px;
        }
        
    }
    &__btn {
        font-weight: 900;
        font-size: 20px;           
        line-height: 24px;
       text-transform: uppercase;
        color: #2E9ADB;
        background: linear-gradient(0deg, #FFFFFF, #FFFFFF);
        border: 4px solid #2E9ADB;
        box-sizing: border-box;
        border-radius: 40px;
        padding: 28px 48px;
    }

}
@media only screen and (max-width: 750px) {
    .coworking {
        &__items {
            margin-top: 0;
            grid-template-columns: 1fr 1fr;
        }
        &__item {
            &-text {
                font-size: 13px;
                line-height: 15px;
            }
        }
        &__btn {
            font-size: 16px;
            line-height: 20px;
            width: 100%;
            padding: 22px 40px;
        }
    }
}
</style>