<template>
<div class="contain">
    <div class="mx-5 grid grid-cols-2 ">
        <div class="left-section text-left ">
            <h2 class="title mb-10">We Are A Creative Digital Agency</h2>
            <p class="paragraph">Dalio started with a vision for building an agency to solve the business problems of the future, and that requires a different model.
                We’re not a branding agency that dabbles in tech, and we’re not a development shop that leaves you hanging when it’s time
                to go to market.
                <br>
                <br>
                We start with human experience and layer in technology and
                marketing to deliver truly integrated digital solutions.
                This unique set of capabilities sets us apart from other agencies
                and positions DIG to help you attack your goals.</p>
                <button class="yellow-button flex items-center ">Contact Us
                <img style="width: 15px; height: 15px" class="ml-2.5" src="../image/turn.svg" alt="">
                </button>
        </div>
        <div class="right-section flex grid grid-cols-2 ml-10">
            <div class="left-image-section ml-10 ">
                <img class="mb-5" src="../image/dg-left-image-1.svg" alt="">
                <img class="left-section-rotate-2 ml-10" src="../image/left-image-bottom.png" alt="">
            </div>
            <div class="right-image-section relative">
                <img class="x-line absolute" src="../image/x-line.svg" alt="">
                <img src="../image/dg-right-image-1.png" alt="">
                <img class="mt-5" src="../image/dg-right-image-2.png" alt="">
                <img src="../image/eclipse-ball.svg" alt="" class="eclipse absolute">
            </div>
        </div>
    </div>
</div>
    <section class="some-values grid grid-cols-4 mx-60">
        <div class="item">
            <p class="title">4.8k</p>
            <p class="text">Job Completed</p>
        </div>
        <div class="item">
            <p class="title">12+</p>
            <p class="text">Industry Experience</p>
        </div>
        <div class="item">
            <p class="title">2.5k+</p>
            <p class="text">World wide clients</p>
        </div>
        <div class="item">
            <p class="title">120+</p>
            <p class="text">Won Awards</p>
        </div>
    </section>
</template>

<script>
export default {
    name: "DigitalAgency"
}
</script>

<style lang="scss" scoped>
*{
    font-family: inter;
}
.contain{
    display: block;
    margin-top: 470px;
    color:white;
}
.some-values{
    padding-bottom: 500px;
    margin-top: 140px;
    .item {
        .title{
            font-style: normal;
            font-size: 48px;
            line-height: 58px;
            font-weight: 700;
            color: #fff;
        }
        .text{
            font-style: normal;
            color:#E0E5F3;
            font-weight: 400;
            text-align: center;
            line-height: 24.2px;
            font-size: 20px;
            opacity: .8;
        }
    }
}
.left-section{
    margin-left: 150px;
    .title{
        width: 440px;
        color: #FFFFFF;
        font-weight: 700;
        font-size: 48px;
        line-height: 58px;
    }
    .paragraph{
        color:#E0E5F3 ;
        font-size: 16px;
        line-height: 30px;
        font-weight: 400;
    }
    .yellow-button{
        color: #0A142F;
        opacity: 1;
        padding: 20px;
        border-radius: 30px;
        background-color: #FFC93E;
        height: 60px;
        margin-top: 48px;
    }
}
.right-section{
    margin-left: 82px;
    .right-image-section{
        margin-top: 60px;
        .x-line{
            opacity: .6;
            top:-60px;
            left: 40px;
        }
        .eclipse{
            top:450px;
            right: 50px;
            z-index: 0;
            opacity: .3;
        }
    }
    }


</style>