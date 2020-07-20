<template>
    <div class="swiper-container">
        <div class="swiper-wrapper">
            <div class="swiper-slide">
                <img class="dolphin1" src="../assets/images/1.3.png">
                <img class="typeface" src="../assets/images/1.4.png"/>

                <div class="bt1" :class="'animate__animated animate__zoomInDown'">
                    <img @click="brand" src="../assets/images/1.5.png" height="40" width="148"/>
                    <img @click="advantage" src="../assets/images/1.6.png" height="40" width="148"/>
                    <img @click="community" src="../assets/images/1.7.png" height="40" width="147"/>
                    <img @click="smart" src="../assets/images/1.8.png" height="40" width="148"/>
                    <img @click="house" src="../assets/images/1.9.png" height="40" width="178"/>
                    <img @click="vr" src="../assets/images/1.10.png" height="40" width="148"/>
                </div>
            </div>
            <div class="swiper-slide">

                <img class="particulars" src="../assets/images/2.2.png" height="290" width="373"/>

                <img class="headline" src="../assets/images/2.1.png" height="242" width="65"/>
                <img class="map" src="../assets/images/2.3.png" height="367" width="446"/>

                <img class="db" src="../assets/images/2.5.png" height="134" width="459"/>

                <img  class="backtrack" @click="backtrack" src="../assets/images/2.4.png" height="40" width="123"/>
            </div>
            <div class="swiper-slide">

                <img class="particulars" src="../assets/images/3.1.png" height="292" width="309"/>
                <img class="dolphin2" src="../assets/images/3.2.png" height="456" width="442"/>
                <img class="certificate" src="../assets/images/3.3.png" height="211" width="607"/>
                <img class="dolphin3" src="../assets/images/3.4.png" height="155" width="344"/>
            </div>
            <div class="swiper-slide">
                <img class="particulars" src="../assets/images/4.2.png" height="268" width="372"/>
                <img class="show" src="../assets/images/4.4.png" height="440" width="641"/>
                <img class="headline" src="../assets/images/4.1.png" height="242" width="65"/>
                <img class="dolphin4" src="../assets/images/4.3.png" height="233" width="224"/>
                <img  class="backtrack" style="bottom: 40%;left: 10%" @click="backtrack" src="../assets/images/2.4.png" height="40" width="123"/>

            </div>
            <div class="swiper-slide">
                <img class="particulars" src="../assets/images/5.1.png" height="192" width="364"/>
                <img class="show" src="../assets/images/5.3.png" height="440" width="641"/>
                <img class="dolphin3" src="../assets/images/3.4.png" height="155" width="344"/>
                <img class="dolphin5" src="../assets/images/5.2.png" height="267" width="482"/>
            </div>
            <div class="swiper-slide">
                <img class="particulars" src="../assets/images/6.1.png" height="192" width="268"/>
                <img class="show" src="../assets/images/6.3.png" height="440" width="640"/>
                <img class="dolphin3" src="../assets/images/3.4.png" height="155" width="344"/>
                <img class="dolphin2" src="../assets/images/3.2.png" height="456" width="442"/>
            </div>
            <div class="swiper-slide">
                <img class="particulars" src="../assets/images/7.1.png" height="226" width="393"/>
                <img class="show" src="../assets/images/7.3.png" height="440" width="641"/>
                <img class="dolphin3" src="../assets/images/3.4.png" height="155" width="344"/>
                <img class="dolphin5" src="../assets/images/5.2.png" height="267" width="482"/>
            </div>
            <div class="swiper-slide">


                <img class="headline" src="../assets/images/8.1.png" height="243" width="65"/>
                <img class="particulars" src="../assets/images/8.2.png" height="257" width="393"/>
                <img class="map" src="../assets/images/8.3.png" height="557" width="507"/>
                <img  class="backtrack" style="bottom: 15%;left: 10%" @click="backtrack" src="../assets/images/2.4.png" height="40" width="123"/>
            </div>
            <div class="swiper-slide">

                <img class="particulars" src="../assets/images/9.1.png" height="260" width="343"/>
                <img class="show" src="../assets/images/9.3.png" height="440" width="641"/>
                <img class="dolphin2" src="../assets/images/3.2.png" height="456" width="442"/>
                <img class="dolphin3" src="../assets/images/3.4.png" height="155" width="344"/>
            </div>
            <div class="swiper-slide">
                <img class="show" src="../assets/images/10.3.png" height="364" width="641"/>
                <img class="particulars" src="../assets/images/10.1.png" height="295" width="404"/>
                <img class="dolphin5" src="../assets/images/5.2.png" height="267" width="482"/>
                <img class="dolphin3" src="../assets/images/3.4.png" height="155" width="344"/>
            </div>
            <div class="swiper-slide">

                <img class="show" src="../assets/images/11.4.png" height="440" width="641"/>
                <img class="particulars" src="../assets/images/11.2.png" height="223" width="403"/>
                <img class="dolphin4" style="top: 40%" src="../assets/images/4.3.png" height="233" width="224"/>
                <img class="dolphin3" src="../assets/images/3.4.png" height="155" width="344"/>
                <img class="headline" src="../assets/images/11.1.png" height="243" width="65"/>
                <img  class="backtrack" style="bottom: 40%;left: 10%" @click="backtrack" src="../assets/images/2.4.png" height="40" width="123"/>
            </div>
            <div class="swiper-slide">
                <img class="show" src="../assets/images/12.3.png" height="440" width="641"/>
                <img class="particulars" src="../assets/images/12.1.png" height="226" width="363"/>
                <img class="dolphin5" src="../assets/images/5.2.png" height="267" width="482"/>
                <img class="dolphin3" src="../assets/images/3.4.png" height="155" width="344"/>
            </div>
            <div class="swiper-slide">
                <img style="width: 30%;height: auto;position: absolute;right: 10%;bottom: 50%"
                     src="../assets/images/3.2.png" height="456" width="442"/>
                <img class="particulars" src="../assets/images/13.1.png" height="225" width="351"/>
                <img class="show" src="../assets/images/12.4.png" height="581" width="641"/>

            </div>

            <div class="swiper-slide">

                <img class="particulars" src="../assets/images/14.2.png" height="188" width="341"/>
                <img class="headline" src="../assets/images/14.1.png" height="295" width="65"/>
                <img class="show" src="../assets/images/14.4.png" height="442" width="641"/>
                <img class="dolphin4" style="top: 40%;" src="../assets/images/4.3.png" height="233" width="224"/>
                <img class="dolphin3" src="../assets/images/3.4.png" height="155" width="344"/>
                <img  class="backtrack" style="bottom: 40%;left: 10%" @click="backtrack" src="../assets/images/2.4.png" height="40" width="123"/>
            </div>
            <div class="swiper-slide">

                <img class="particulars" src="../assets/images/15.1.png" height="217" width="319"/>
                <img class="show" src="../assets/images/15.3.png" height="440" width="641"/>
                <img class="dolphin3" src="../assets/images/3.4.png" height="155" width="344"/>
                <img class="dolphin2" src="../assets/images/3.2.png" height="456" width="442"/>
                <img class="dolphin3" src="../assets/images/3.4.png" height="155" width="344"/>


            </div>
            <div class="swiper-slide">
                <img class="dolphin3" src="../assets/images/3.4.png" height="155" width="344"/>
                <img class="headline" src="../assets/images/16.1.png" height="282" width="65"/>
                <img class="model" src="../assets/images/16.2.png" height="360" width="400"/>
                <img class="brief"  src="../assets/images/16.3.png" height="235" width="482"/>
                <img class="dolphin3" src="../assets/images/3.4.png" height="155" width="344"/>
                <img  class="backtrack" style="bottom: 10%;left: 70%" @click="backtrack" src="../assets/images/2.4.png" height="40" width="123"/>

            </div>
            <div class="swiper-slide">
                <img class="model" src="../assets/images/20.2.png" height="376" width="400"/>
                <img class="details"
                     src="../assets/images/20.3.png" height="244" width="449"/>
                <img class="headline" @click="see('http://720yun.com/t/49vkue19zrl?scene_id=38553456')" src="../assets/images/20.1.png" height="404" width="83"/>
                <img  class="backtrack" style="bottom: 5%;left: 76%" @click="backtrack" src="../assets/images/2.4.png" height="40" width="123"/>
            </div>
        </div>
    </div>
</template>

<script>

    import '../assets/css/swiper.min.css';
    import Swiper from 'swiper';

    export default {
        name: "slideshow",
        data() {
            return {
                slideId: 0,
                switch: true,
                swiper: null,


            }
        },
        mounted() {


            this.swiper = new Swiper('.swiper-container', {
                direction: 'vertical',
                followFinger: false,
                speed: 1000,
                mousewheel: true,
                pagination: {
                    el: '.swiper-pagination',
                    clickable: true,
                },
                on: {
                    init(swiper) {
                        let slide = this.slides.eq(0);
                        slide.addClass('ani-slide');
                    },
                    //可视页面没出现时动画的位置
                    transitionStart() {
                        for (let i = 0; i < this.slides.length; i++) {
                            let slide = this.slides.eq(i);
                            slide.removeClass('ani-slide');
                        }
                    },
                    //可视页面出现的动画
                    transitionEnd() {
                        let slide = this.slides.eq(this.activeIndex);
                        slide.addClass('ani-slide');

                    },
                }
            });
        },
        watch: {},
        methods: {
            brand() {
                this.swiper.slideTo(1, 1, false);
            },
            advantage() {
                this.swiper.slideTo(3, 1, false);

            },
            community() {
                this.swiper.slideTo(7, 1, false);

            },
            smart() {
                this.swiper.slideTo(10, 1, false);

            },
            house() {
                this.swiper.slideTo(13, 1, false);

            },
            vr() {
                this.swiper.slideTo(15, 1, false);

            },
            backtrack(){
                this.swiper.slideTo(0, 1, false);
            },
            see(e){
                window.location.href = e
             },
        },
    }
</script>

<style scoped lang="scss">
    body {
        background: #eee;
        font-family: Helvetica Neue, Helvetica, Arial, sans-serif;
        font-size: 14px;
        color: #000;
        margin: 0;
        padding: 0;
    }

    .swiper-wrapper {
        transition-delay: .3s;
    }

    .swiper-container {
        width: 100vw;
        height: 100vh;

    }

    .swiper-slide {
        /*text-align: center;*/
        font-size: 18px;
        background: #fff;

        /* Center slide text vertically */
        display: -webkit-box;
        display: -ms-flexbox;
        display: -webkit-flex;
        /*display: flex;*/
        -webkit-box-pack: center;
        -ms-flex-pack: center;
        -webkit-justify-content: center;
        /*justify-content: center;*/
        -webkit-box-align: center;
        -ms-flex-align: center;
        -webkit-align-items: center;
        /*align-items: center;*/
    }

    .dolphin1 {
        top: 36%;
        width: 85%;
        position: absolute;
    }

    .dolphin2 {
        top: 25%;
        right: 5%;
        width: 65%;
        height: auto;
        position: absolute;
    }

    .dolphin3 {
        bottom: 0;
        left: 0;
        width: 40%;
        height: auto;
        position: absolute;
    }

    .dolphin4 {
        top: 45%;
        right: 15%;
        width: 40%;
        height: auto;
        position: absolute;

    }

    .dolphin5 {
        top: 45%;
        right: 5%;
        width: 70%;
        height: auto;
        position: absolute;

    }

    .show {

        left: 0;
        width: 100%;
        height: auto;
        position: absolute;
        opacity: 1;

    }

    .typeface {
        top: 68%;
        width: 85%;
        position: absolute;
    }

    .bt1 {
        position: absolute;
        top: 76%;
        justify-content: center;
        height: 40%;


        img {
            /*vertical-align: top;*/
            width: 28%;
            height: auto;
            margin: 4% 1% 0 3.5%;
        }
    }

    .particulars {
        position: absolute;
        top: 20%;
        left: 5%;
        width: 60%;
        height: auto;

    }

    .model {
        position: absolute;
        top: 20%;
        left: 12%;
        width: 65%;
        height: auto;

    }

    .swiper-slide .dolphin3 {
        width: 10%;
        height: auto;
        transition: all .3s;
    }

    .ani-slide .dolphin3 {
        transform: translate(0, 0) rotate(0deg);
        opacity: 1;
        width: 40%;
        height: auto;

    }

    .swiper-slide .particulars {
        opacity: 0;
        transform-origin: left bottom;
        -webkit-animation: rotateOutUpLeft 1s;
        animation: rotateOutUpLeft 1s;
    }
    @keyframes rotateOutUpLeft {
        from {
            opacity: 1;
        }

        to {
            transform: rotate3d(0, 0, 1, -45deg);
            opacity: 0;
        }
    }

    .rotateOutUpLeft {
        animation-name: rotateOutUpLeft;

    }

    .ani-slide .particulars {
        -webkit-animation: rotateInDownLeft 1s;
        animation: rotateInDownLeft 1s;
        transform-origin: left bottom;
        opacity: 1;
    }

    @keyframes rotateInDownLeft {
        from {
            transform: rotate3d(0, 0, 1, -45deg);
            opacity: 0;
        }

        to {
            transform: translate3d(0, 0, 0);
            opacity: 1;
        }
    }

    .rotateInDownLeft {
        animation-name: rotateInDownLeft;

    }

    .rotateInUpLeft {
        animation-name: rotateInUpLeft;
        transform-origin: left bottom;
    }

    .headline {
        position: absolute;
        top: 20%;
        right: 5%;
        width: 10%;
        height: auto;

    }

    .map {
        position: absolute;
        top: 48%;
        right: 18%;
        width: 70%;
        height: auto;

    }
    .brief{
        position: absolute;
        top: 62%;
        right: 7%;
        width: 80%;
        height: auto;

    }

    .db {
        position: absolute;
        bottom: 4%;
        width: 80%;
        height: auto;
    }

    .certificate {
        position: absolute;
        bottom: 20%;
        width: 90%;
        height: auto;

    }

    .swiper-slide:nth-child(1) {
        background: url(../assets/images/3.png) no-repeat;
        background-size: 100% 100%;

    }


    .swiper-slide:nth-child(n+2):nth-child(-n+17) {
        background: url(../assets/images/4.png) no-repeat;
        background-size: 100% 100%;

    }

    .swiper-slide p {
        transform: translateX(-200px);
        opacity: 0;
        transition: all .4s;
    }

    .ani-slide p {
        transform: translateX(0);
        opacity: 1;
    }

    .swiper-slide .dolphin1, .db {
        transform: translate(-400px, 200px) rotate(9deg);
        opacity: 0;
        transition: all .8s;
    }

    .ani-slide .dolphin1, .db {
        transform: translate(0, 0) rotate(0deg);
        opacity: 1;
    }

    .swiper-slide .db {
        transform: translate(-400px, 200px) rotate(9deg);
        opacity: 0;
        transition: all .8s;
    }

    .ani-slide .db {
        transform: translate(0, 0) rotate(0deg);
        opacity: 1;
    }

    .swiper-slide .headline {

        animation: turn 1s linear 1;
    }

    @keyframes turn {
        0% {
            -webkit-transform: rotate(0deg) translate(0px, 100px);
        }
        25% {
            -webkit-transform: rotate(90deg) translate(0px, 75px);
        }
        50% {
            -webkit-transform: rotate(180deg) translate(0px, 50px);
        }
        75% {
            -webkit-transform: rotate(270deg) translate(0px, 25px);
        }
        100% {
            -webkit-transform: rotate(360deg) translate(0, 0);
        }
    }

    .ani-slide .headline {

        animation: rotate .5s linear 4;
    }

    @keyframes shadow {
        0%, 100% {
            transform: scaleX(1);
        }
        50% {
            transform: scaleX(1.2);
        }
    }

    @keyframes rotate {
        0% {
            transform: translateY(0);
        }
        25% {
            transform: translateY(10px);
        }
        50% {
            transform: translateY(25px) scale(1.1, 0.9);

        }
        75% {
            transform: translateY(10px);
        }
        100% {
            transform: translateY(0);
        }
    }

    .swiper-slide .show {
        bottom: -200px;
        opacity: 0;
        transition: all 0.5s ease 1s;

    }
    .ani-slide .show {
        bottom: 0;
        opacity: 1;
    }


    .swiper-slide .certificate {
        opacity: 0;

    }

    .ani-slide .certificate {
        -webkit-animation: zoomInUp 0.7s;
        animation: zoomInUp 0.7s;
        opacity: 1;
    }

    @keyframes zoomInUp {
        from {

            transform: scale3d(0.1, 0.1, 0.1) translate3d(0, 1000px, 0);
            animation-timing-function: cubic-bezier(0.55, 0.055, 0.675, 0.19);
        }

        60% {
            opacity: 1;
            transform: scale3d(0.475, 0.475, 0.475) translate3d(0, -20%, 0);
            animation-timing-function: cubic-bezier(0.175, 0.885, 0.32, 1);
        }
    }

    .details {
        position: absolute;
        bottom: 5%;
        width: 90%;
        height: auto;
        left: 5%;

    }
    .swiper-slide .details {
        opacity: 0;

    }

    .ani-slide .details {
        -webkit-animation: fadenum 2s;
        animation: fadenum 2s;
        opacity: 1;

    }
    @-webkit-keyframes fadenum{

        0%{opacity: 0;}

        100%{opacity: 1;}

    }


    .swiper-slide .brief {
        opacity: 0;

    }

    .ani-slide .brief {
        -webkit-animation: fadenum 2s;
        animation: fadenum 2s;
        opacity: 1;

    }
    @-webkit-keyframes fadenum{

        0%{opacity: 0;}

        100%{opacity: 1;}

    }
   .backtrack{
       position: absolute;
       width: 20%;
       left: 15%;
       bottom: 20%;
       height:auto;
   }
    .swiper-slide .backtrack {
        opacity: 0;

    }

    .ani-slide .backtrack {
        -webkit-animation: fadenum 2.5s;
        animation: fadenum 2.5s;
        opacity: 0.8;

    }
    @-webkit-keyframes fadenum{

        0%{opacity: 0;}

        100%{opacity: 0.8;}

    }
</style>
