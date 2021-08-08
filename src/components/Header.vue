<template>
    <header class="header">
        <div class="container header__container">
            <router-link class="logo" to="/"><img src="../assets/logo.png" alt=""></router-link>
            <div class="header__items">
                <nav class="nav d-none">
                    <router-link class="nav__item" to="/">вебмастерам</router-link>
                    <router-link class="nav__item" to="/рекламодателям">рекламодателям</router-link>
                </nav>
                <div class="signing">
                    <button class="signing__btn">вход</button>
                    <span class="signing__span">|</span>
                    <button class="signing__btn d-none">регистрация</button>
                </div>
                <form class="form">
                <input
                    class="form__input"
                    type="checkbox"
                    name="opt"
                    id="opt1"
                    checked="checked"
                />
                <label class="form__lable active" for="opt1">RU</label>
                <input class="form__input" type="checkbox" name="opt" id="opt2" />
                <label class="form__lable active" for="opt2">EN</label>
                </form>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header",
}
</script>

<style lang="scss">
.header {
    padding: 16px 0;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    background: white;
    box-shadow: 0px 1px 4px #4eaae0;
    z-index: 3;
    &__container {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    &__items {
        display: flex;
        align-items: center;
        gap: 80px;

        .nav {
            display: flex;
            gap: 50px;

            &__item {
                font-weight: bold;
                font-size: 13px;
                line-height: 16px;
                text-transform: uppercase;
                color: #565656;
            }
            .router-link-exact-active.router-link-active {
                &::before {
                        content: '';
                        background: #2E9ADB;
                        height: 5px;
                        width: 7%;
                        display: block;
                        margin: auto;
                        position: absolute;
                        top: 0;
                }
            }
        }
        .signing {
            display: flex;
            align-items: center;
            gap: 10px;

            &__btn {
                font-weight: 800;
                font-size: 13px;
                line-height: 16px;
                text-transform: uppercase;
                color: #55B570;
                border: none;
                outline: none;
                background: white;
                
            }

        }
        .form {
            background: #f9f9f9;
            border: 1px solid #ebebeb;
            box-sizing: border-box;
            border-radius: 14px;
            height: 30px;
            width: 78px;
            display: flex;
            align-items: center;
            justify-content: space-around;

            &__input[type="checkbox"] {
                display: none;
            }

            &__lable {
                font-style: normal;
                font-weight: bold;
                font-size: 11px;
                line-height: 13px;
                display: flex;
                align-items: center;
                text-align: center;
                color: #797979;
                padding: 8px 10px;
                border-radius: 14px;
                cursor: pointer;
            }

            &__lable:active{
                padding: 8px 13.5px;
                color: #fff;
                background-color: #4eaae0;
                // transition: all 0.35s ease-in-out;
            }
        }
        
    }
}
@media only screen and (max-width: 750px) {
    .d-none {
        display: none;
    }
    .header {
        &__items {
            position: relative;
            gap: 8px;
            .nav {
                display: none;
            }
        }
    }
}
</style>