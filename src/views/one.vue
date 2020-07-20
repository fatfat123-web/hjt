<template>

    <div class="container animate__animated"
         :class="animateEnd ? '' : 'animate__fadeOut'">

    </div>
<!--<div>22222222222222</div>-->
</template>

<script>


    export default {
        name: "one",
        data(){
            return{
                animateEnd: true,
                animate: true,
            }

        },
        components: {
  
        },
        mounted() {
            this.animate = false
            setTimeout(() => {

                this.animateEnd = false
                setTimeout(() => {
                    this.$router.push('two')

                }, 400)
            }, 3500)
        },
    }
</script>

<style scoped lang="scss">
    .container {
        width: 100%;
        height: 100%;
        background: url(../../assets/images/1.png) no-repeat bottom;
        background-size: 100% 100%;
    }

</style>
