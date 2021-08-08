<template>
    <section class="intro">
        <Particles class="particles" id="tsparticles" :particlesInit="particlesInit" :particlesLoaded="particlesLoaded"
            :options="option" />
        <div class="container intro__container">
            <h1 class="intro__title">Мобильная партнерская сеть</h1>
            <p class="intro__text">Только рабочие офферы от прямых рекламодателей</p>

            <div class="intro__details">
                <div class="intro__detail b-right b-bottom">
                    <h2 class="intro__detail-title">300+</h2>
                    <p class="intro__detail-text">офферов по всему миру</p>
                </div>
                <div class="intro__detail b-bottom br-none">
                    <h2 class="intro__detail-title">70+</h2>
                    <p class="intro__detail-text">активных рекламодателей</p>
                </div>
                <div class="intro__detail b-right">
                    <h2 class="intro__detail-title">6 лет</h2>
                    <p class="intro__detail-text">в аффилейт маркетинге</p>
                </div>
                <div class="intro__detail">
                    <h2 class="intro__detail-title">10.000+</h2>
                    <p class="intro__detail-text">конверсий в день</p>
                </div>
            </div>
            <div class="intro__boxes">
                <div class="intro__box">
                    <p class="intro__box-text">Я пользователь соцсетей, блогер, владелец сайта или арбитражник и хочу
                        сотрудничать с топовыми мировыми брендами.</p>
                    <button class="intro__box-btn">веб-мастерам
                        <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <g clip-path="url(#clip0)">
                                <path
                                    d="M10.553 19.7709C10.5532 19.7706 10.5535 19.7704 10.5538 19.7702L14.6163 15.688C14.9206 15.3821 14.9195 14.8875 14.6136 14.5831C14.3078 14.2787 13.8131 14.2799 13.5088 14.5857L10.7813 17.3265L10.7813 0.78125C10.7813 0.349765 10.4315 -1.92866e-07 10 -2.11727e-07C9.56852 -2.30588e-07 9.21875 0.349765 9.21875 0.78125L9.21875 17.3264L6.49125 14.5857C6.18688 14.2799 5.69223 14.2788 5.38641 14.5831C5.08051 14.8875 5.07945 15.3822 5.38375 15.688L9.44625 19.7702C9.44649 19.7704 9.44676 19.7706 9.44699 19.7709C9.75238 20.0769 10.2486 20.0759 10.553 19.7709Z"
                                    fill="white" />
                            </g>
                            <defs>
                                <clipPath id="clip0">
                                    <rect width="20" height="20" fill="white" transform="translate(20) rotate(90)" />
                                </clipPath>
                            </defs>
                        </svg>
                    </button>
                </div>
                <div class="intro__box">
                    <p class="intro__box-text">Я пользователь соцсетей, блогер, владелец сайта или арбитражник и хочу
                        сотрудничать с топовыми мировыми брендами.</p>
                    <button class="intro__box-btn intro__box-btn_color">рекламодателю
                        <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <g clip-path="url(#clip0)">
                            <path d="M19.7709 9.44699C19.7706 9.44676 19.7704 9.44648 19.7702 9.44625L15.688 5.38375C15.3821 5.07941 14.8875 5.08054 14.5831 5.3864C14.2787 5.69222 14.2799 6.18687 14.5857 6.49125L17.3265 9.21875H0.78125C0.349766 9.21875 0 9.56851 0 10C0 10.4315 0.349766 10.7812 0.78125 10.7812H17.3264L14.5857 13.5087C14.2799 13.8131 14.2788 14.3078 14.5831 14.6136C14.8875 14.9195 15.3822 14.9205 15.688 14.6162L19.7702 10.5537C19.7704 10.5535 19.7706 10.5532 19.7709 10.553C20.0769 10.2476 20.0759 9.75137 19.7709 9.44699Z" fill="white"/>
                            </g>
                            <defs>
                            <clipPath id="clip0">
                            <rect width="20" height="20" fill="white"/>
                            </clipPath>
                            </defs>
                        </svg>
                    </button>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {

        name: "Intro",

        data() {
            return {
                option: {
                    // background: {
                    // color: {
                    //     value: '#333'
                    // }
                    // },
                    fpsLimit: 60,
                    interactivity: {
                        detectsOn: 'canvas',
                        events: {
                            onClick: {
                                enable: true,
                                mode: 'push'
                            },
                            onHover: {
                                enable: true,
                                mode: 'repulse'
                            },
                            resize: true
                        },
                        modes: {
                            bubble: {
                                distance: 400,
                                duration: 2,
                                opacity: 0.8,
                                size: 40
                            },
                            push: {
                                quantity: 4
                            },
                            repulse: {
                                distance: 200,
                                duration: 0.4
                            }
                        }
                    },
                    particles: {
                        color: {
                            value: '#ffffff'
                        },
                        links: {
                            color: '#ffffff',
                            distance: 150,
                            enable: true,
                            opacity: 0.5,
                            width: 1
                        },
                        collisions: {
                            enable: true
                        },
                        move: {
                            direction: 'none',
                            enable: true,
                            outMode: 'bounce',
                            random: false,
                            speed: 6,
                            straight: false
                        },
                        number: {
                            density: {
                                enable: true,
                                value_area: 800
                            },
                            value: 80
                        },
                        opacity: {
                            value: 0.5
                        },
                        shape: {
                            type: 'circle'
                        },
                        size: {
                            random: true,
                            value: 5
                        }
                    },
                    detectRetina: true
                }
            }
        }
    }
</script>

<style lang="scss">
    .intro {
        background-image: url('../assets/bg.png');
        height: 100%;
        width: 100%;
        margin-top: 80px;
        padding-top: 200px;
        background-size: cover;
        background-repeat: no-repeat;
        height: 900px;

        &__container {
            text-align: center;
        }

        .particles {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            z-index: 1;
        }

        &__title {
            font-weight: 900;
            font-size: 60px;
            line-height: 75px;
            text-transform: uppercase;
            color: #FFFFFF;
        }

        &__text {
            font-weight: 500;
            font-size: 20px;
            line-height: 24px;
            color: #FFFFFF;
            margin-bottom: 150px;
        }

        &__details {
            display: flex;
            align-items: center;
        }

        &__detail:not(:last-child) {
            border-right: 1px solid rgba(255, 255, 255, 0.25);
        }

        &__detail {
            text-align: center;
            flex-basis: 25%;
            padding: 60px 0;

            &-title {
                font-weight: 800;
                font-size: 40px;
                line-height: 49px;
                color: #FFFFFF;
            }

            &-text {
                font-weight: 500;
                font-size: 16px;
                line-height: 19px;
                color: #FFFFFF;
            }
        }

        &__boxes {
            display: flex;
            background: #FFFFFF;
            box-shadow: 0px 20px 80px rgba(0, 0, 0, 0.08);
            border-radius: 8px;
            // height: 300px;

        }
        &__box:not(:last-child) {
            border-right: 1px solid rgba(10, 10, 10, 0.25);
        }
        &__box {
            text-align: center;
            flex-basis: 50%;
            padding: 58px 50px;
        

            &-text {
                font-weight: 500;
                font-size: 16px;
                line-height: 24px;
                color: #000000;
                // padding-top: 58px;
                // padding: 58px 50px 0;
                margin-bottom: 32px;
            }

            &-btn {
                font-weight: 900;
                font-size: 20px;
                line-height: 24px;
                text-transform: uppercase;
                color: #FFFFFF;
                display: flex;
                align-items: center;
                gap: 18px;
                background: #2E9ADB;
                box-shadow: 0px 10px 20px rgba(78, 170, 224, 0.35);
                border-radius: 40px;
                padding: 28px 38px;
                margin: auto;
                border: none;
                outline: none;
                &_color {
                    background: #55B570;
                }
            }
        }
    }

    @media only screen and (max-width: 750px) {
        .b-right {
            border-right: 2px solid rgba(255, 255, 255, 0.25);
        }
        .b-bottom {
            border-bottom: 2px solid rgba(255, 255, 255, 0.25);
        }
        .br-none {
            border-right: none !important;
        }
        .intro {
            height: auto;
            margin-top: 0;
            .particles {
                bottom: 0;
            }
            &__title {
                font-size: 32px;
                line-height: 40px;
            }
            &__text {
                font-size: 16px;
                line-height: 19px;
                margin-bottom: 0;
            }
            &__details {
                display: grid;
                grid-template-columns: 1fr 1fr;
            }
            &__detail {
                padding: 30px 0;
                &-title {
                    font-size: 30px;
                    line-height: 37px;
                }
                &-text {
                    font-size: 13px;
                    line-height: 18px;
                }
            }
            &__boxes {
                flex-direction: column;
                z-index: 2;
            }
            &__box:not(:last-child) {
                border: none;
                border-bottom: 2px solid #F3F3F3;

                
            }
            &__box {
                &-btn {
                    padding: 18px 28px;
                    font-size: 16px;
                }
            }
            
        }
    }
</style>