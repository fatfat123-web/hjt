<template>
    <div class="container">
        <div style="position: fixed;top:3.7%;right:23.1%;z-index: 999;">
            <div class="rotation">{{isPlay ? '关音乐' : '开音乐'}}</div>
            <div class="loader1" @click="pause(true)">
                <div class="loop">
                    <div class="ring"></div>
                </div>
                <div class="loop">
                    <div class="ring"></div>
                </div>
            </div>
            <audio ref="music" id="music" src="../assets/music/cn.mp3" loop="loop" preload autoplay="autoplay"></audio>
        </div>
        <router-view/>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                music: false,
                list: [
                    require('../assets/images/hty.gif'),
                    require('../assets/images/1.png'),
                    require('../assets/images/1.1.png'),
                    require('../assets/images/1.2.png'),
                    require('../assets/images/1.3.png'),
                    require('../assets/images/1.4.png'),
                    require('../assets/images/1.5.png'),
                    require('../assets/images/1.6.png'),
                    require('../assets/images/1.7.png'),
                    require('../assets/images/1.8.png'),
                    require('../assets/images/1.9.png'),
                    require('../assets/images/1.10.png'),
                    require('../assets/images/2.png'),
                    require('../assets/images/2.1.png'),
                    require('../assets/images/2.2.png'),
                    require('../assets/images/2.3.png'),
                    require('../assets/images/2.4.png'),
                    require('../assets/images/2.5.png'),
                    require('../assets/images/3.png'),
                    require('../assets/images/3.1.png'),
                    require('../assets/images/3.2.png'),
                    require('../assets/images/3.3.png'),
                    require('../assets/images/3.4.png'),
                    require('../assets/images/4.png'),
                    require('../assets/images/4.1.png'),
                    require('../assets/images/4.2.png'),
                    require('../assets/images/4.3.png'),
                    require('../assets/images/4.4.png'),
                    require('../assets/images/5.1.png'),
                    require('../assets/images/5.2.png'),
                    require('../assets/images/5.3.png'),
                    require('../assets/images/6.1.png'),
                    require('../assets/images/6.3.png'),
                    require('../assets/images/7.1.png'),
                    require('../assets/images/7.3.png'),
                    require('../assets/images/8.1.png'),
                    require('../assets/images/8.2.png'),
                    require('../assets/images/8.3.png'),
                    require('../assets/images/9.1.png'),
                    require('../assets/images/9.3.png'),
                    require('../assets/images/10.1.png'),
                    require('../assets/images/10.3.png'),
                    require('../assets/images/11.1.png'),
                    require('../assets/images/11.2.png'),
                    require('../assets/images/11.4.png'),
                    require('../assets/images/12.1.png'),
                    require('../assets/images/12.3.png'),
                    require('../assets/images/12.4.png'),
                    require('../assets/images/13.1.png'),
                    require('../assets/images/14.1.png'),
                    require('../assets/images/14.2.png'),
                    require('../assets/images/14.4.png'),
                    require('../assets/images/15.1.png'),
                    require('../assets/images/15.2.png'),
                    require('../assets/images/15.3.png'),
                    require('../assets/images/16.1.png'),
                    require('../assets/images/16.2.png'),
                    require('../assets/images/16.3.png'),
                    require('../assets/images/17.1.png'),
                    require('../assets/images/18.1.png'),
                    require('../assets/images/19.1.png'),
                    require('../assets/images/20.1.png'),
                    require('../assets/images/20.2.png'),
                    require('../assets/images/20.3.png'),
                    require('../assets/images/22.1.png'),
                    require('../assets/images/22.2.png'),
                    require('../assets/music/cn.mp3'),


                ],
                isPlay: false,
            }
        },
        created() {
            let count = 0;
            for (let item of this.list) {
                let img = new Image()
                img.src = item;
                count++
                if (count === 67) {
                    this.$router.push('/one')
                }
            }
        },
        // computed: {
        //     isPlay() {
        //         return this.$isPlay
        //     }
        // },
        watch: {
            isPlay(val) {
                // console.log(val)
            }
        },
        mounted() {
            this.$EventBus.$on('isPlay', data => {
                this.isPlay = data;
            })
            // this.autoPlayAudio();

        },
        methods:{

            pause(val) {

                // console.log(this.$refs.music)
                if (this.$refs.music !== null) {
                    //检测播放是否已暂停.this.$refs.music.paused 在播放器播放时返回false.
                    // console.log(this.$refs.music.paused);
                    if (this.$refs.music.paused) {
                        this.$refs.music.play();// 这个就是播放
                        this.isPlay= true
                        // console.log(this.music)

                    } else {
                        if (val) {
                            this.$refs.music.pause();// 这个就是暂停
                            this.isPlay = false
                            // console.log(this.music)
                        }
                    }
                }
            },
            autoPlayAudio() {
                //把this的指向给存了起来，使得try里面的pause调用上面的pause方法
                const _this = this
                try {
                    WeixinJSBridge.invoke('WeixinJSBridgeReady', {}, function (e) {
                        _this.pause()
                    });
                } catch (e) {
                    _this.pause()
                }
            },
        },
    }
</script>

<style scoped lang="scss">
    .container {
        width: 100vw;
        height: 100vh;
    }
    .rotation {

        color: white;
        font-weight: 300;
        width: 5em;
        height: 5em;
        font-size: 11px;
        display: flex;
        align-items: center;
        justify-content: center;
        top: 9%;
        left: 5%;
        position: fixed;
        letter-spacing: 2px
    }
    .fontone {
        letter-spacing: 2px;
        font-weight: 500;
        position: absolute;
        font-size: 0.4rem;
        top: 47%;
        color: white;
        transform: rotate(90deg);
        -ms-transform: rotate(90deg);
        -moz-transform: rotate(90deg);
        -webkit-transform: rotate(90deg);
        -o-transform: rotate(90deg);
        filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=1);
        z-index: 2;
    }

    .fontone:before {
        content: '';
        width: 0.2rem;
        height: 0.2rem;
        position: absolute;
        top: 12%;
        left: -15%;
        border: 0.1rem solid #ff9a9f;
        border-radius: 50%;
    }

    .fontone:after {
        content: '';
        width: 0.2rem;
        height: 0.2rem;
        position: absolute;
        top: 12%;
        left: 103%;
        border: 0.1rem solid #ff9a9f;
        border-radius: 50%;
    }
    .loader1 {

        width: 5em;
        height: 5em;
        font-size: 11px;
        display: flex;
        align-items: center;
        justify-content: center;
        top: 9%;
        left: 5%;
        position: fixed;
        letter-spacing: 1px;
        color: white;
        border: 1px dotted pink;
        border-radius: 50%;
    }

    .loader1:active {
        background: yellow;
        opacity: 0.5;
        box-shadow: 5px 5px 20px 10px rgba(255, 255, 0, 0.5)
    }

    .loader1 .loop {
        position: absolute;
        border-radius: 50%;
        border-style: solid;
        animation: animate2 3s linear infinite;
    }

    .loader1 .loop:nth-child(1) {
        width: 100%;
        height: 100%;
        color: gold;
        border-color: currentColor transparent transparent currentColor;
        border-width: 0.2em 0.2em 0 0;
        --deg: -45deg;
        animation-direction: normal;
    }

    .loader1 .loop:nth-child(2) {
        width: 70%;
        height: 70%;
        color: lime;
        border-color: currentColor currentColor transparent transparent;
        border-width: 0.2em 0 0 0.2em;
        --deg: -135deg;
        animation-direction: reverse;
    }

    .loader1 .loop .ring {
        position: absolute;
        width: 50%;
        height: 0.1em;
        top: 50%;
        left: 50%;
        background-color: transparent;
        transform: rotate(var(--deg));
        transform-origin: left;
    }

    .loader1 .loop .ring::before {
        position: absolute;
        top: -0.5em;
        right: -0.5em;
        content: '';
        width: 1em;
        height: 1em;
        background-color: currentColor;
        border-radius: 50%;
        box-shadow: 0 0 2em,
        0 0 4em,
        0 0 6em,
        0 0 8em,
        0 0 10em,
        0 0 0 0.5em rgba(255, 255, 0, 0.1);
    }

    @keyframes animate2 {
        to {
            transform: rotate(1turn);
        }
    }
</style>
