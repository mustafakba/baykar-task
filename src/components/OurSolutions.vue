<template>
<section class="our-solution w-full">
    <div class="container flex ">
        <div class="left-section relative">
            <img class="eclipse absolute" src="../image/eclipse-ball.svg" alt="">
            <img class="our-solution-image absolute" src="../image/oursolutions.png" alt="">
            <img class="dots absolute" src="../image/dots.svg" alt="">
        </div>
        <div class="right-section ">
            <h2 class="right-section-title">Our Solution Approach</h2>
            <div class="item flex">
                <div class="img">
                    <img style="min-width: 25px!important; min-height: 25px!important;" src="../image/lucide_check-circle.svg" alt="">
                </div>
                <div class="item-inner">
                    <div class="title">Data Analysis with problem factor</div>
                    <p class="title-inner">Delivering the spatial expertise of the largest, most sophisticated performance marketing agencies, while providing intimate, boutique-like support.</p>
                </div>
            </div>
            <div class="item flex">
                <div class="img">
                    <img style="min-width: 25px!important; min-height: 25px!important;" src="../image/lucide_check-circle.svg" alt="">
                </div>
                <div class="item-inner">
                    <div class="title">Functionality solution for users</div>
                    <p class="title-inner">Delivering the spatial expertise of the largest, most sophisticated performance marketing agencies.</p>
                </div>
            </div>
            <div class="item flex">
                <div class="img">
                    <img style="min-width: 25px!important; min-height: 25px!important;" src="../image/lucide_check-circle.svg" alt="">
                </div>
                <div class="item-inner">
                    <div class="title">Latest technology enabled</div>
                    <p class="title-inner">Technology the spatial expertise of the largest, most sophisticated performance marketing agencies, while providing intimate, boutique-like support.</p>
                </div>
            </div>
        </div>
    </div>
</section>
</template>

<script>
export default {
    name: "OurSolutions"
}
</script>

<style lang="scss" scoped>
*{
    font-family: inter;

}
.our-solution{
    margin-top: 120px;
    height: 850px;
}
.left-section{
    flex-basis: 40%;
    height: 850px;
    background-color: #FFC93E;
    .eclipse{
        top: 50px;
        right:-190px;
    }
    .dots{
        bottom: 100px;
        left: 100px;
    }
   .our-solution-image{
       margin-left: 130px;
       margin-top: 100px;
       z-index: 999;
   }
}
.right-section{

    display: flex;
    justify-content: center;
    flex-direction: column;
    padding-left: 250px;
    flex-basis: 60%;
    width: 100%;
    height: 850px;
    background-color: #2c3e50;
    .right-section-title{
        margin-bottom: 50px;
        font-style: normal;
        font-weight: 700;
        font-size: 48px;
        line-height:58px;
        color: #FFFFFF;
        text-align: left;

    }
    .item{
        margin-bottom: 42px;
        max-width: 536px;
        display: flex;
        align-items: flex-start;

        .item-inner{
            text-align: left;
            margin-left: 22.5px;
            .title{
                margin-bottom: 18px;
                font-style: normal;
                font-weight: 700;
                font-size: 24px;
                line-height: 29px;
                color: #FFFFFF;
            }
            .title-inner{
                font-style: normal;
                font-weight: 400;
                font-size: 16px;
                line-height: 30px;
                /* or 188% */


                color: #E0E5F3;
            }
        }
    }
}
</style>