<template>
<!--    NAVBAR START-->
    <navbar>
        <div class="cont flex items-center justify-evenly py-5 mr-20">
            <div style="margin-top: 5px; margin-right: 50px" class="logo py-2.5 ">
                <img class="cursor-pointer " src="../image/dalio.svg" alt="">
            </div>
            <div class="lines absolute">
                <img src="../image/left-background-lines.svg" alt="">
            </div>
            <div class="eclipse absolute">
                <img src="../image/eclipse-ball.svg" alt="">
            </div>
            <div class="eclipse-star absolute">
                <img src="../image/star.svg" alt="">
            </div>
            <div class="menu-items">
                <a href="#">About Us</a>
                <a href="#">What We Do </a>
                <a href="#">Our work</a>
                <a href="#">Blog</a>
                <a href="#">Say hi</a>
            </div>
            <div class="menu-icon cursor-pointer relative">
                <img src="../image/menu.svg" alt="">
                <img class="menu-star absolute" src="../image/star.svg" alt="">
            </div>
        </div>
    </navbar>
<!--    NAVBAR END -->

<!--MAIN SECTION START-->
    <section class="relative mr-5" id="main">
        <div class="title mr-20">
            <h2 class="relative digital">Digital
            <img class="long-line  absolute" src="../image/long-lines.svg" alt="">
            </h2>
            <div class="absolute world-class flex items-center justify-center ">
                <img class="relative" src="../image/border.svg" alt="">
                <span class="rotate-text absolute">World Class</span>
                <img class="relative rotate-lines" src="../image/group-line.svg" alt="">
            </div>
            <h2 class="title agency  relative">Agency
                <div class="right-image absolute">
                    <div class="right-star relative">
                        <img class=" right-image ml-2.5" src="../image/homepage-right.svg" alt="">
                        <img class="absolute right-image-star" src="../image/star.svg" alt="">
                        <img class="absolute right-image-bottom-circle" src="../image/right-circle.svg" alt="">
                    </div>
                </div>
            </h2>
        </div>
        <div class="explain">
            <p class="explain-text">Full-service design support that growing B2B companies need. World leading agency.</p>
            <div class="our-project flex relative">
                <button class="yellow-button flex items-center ">Our Projects
                    <img style="width: 15px; height: 15px" class="ml-2.5" src="../image/turn.svg" alt="">
                </button>
                <img class="absolute left-image" src="../image/homepage-left-photo.svg" alt="">
                <img class="eclipse" src="../image/eclipse-ball.svg" alt="">

            </div>
        </div>

    </section>
<!--MAIN SECTION END-->

<!--    SCROLL SECTION START-->
    <section class="scroll-section">
        <div class="scroll-down absolute flex items-center justify-center flex-col">
            <span class="rotate-scroll">Scroll Down</span>
            <img class="scroll-img" src="../image/scroll-down.svg" alt="">
        </div>
    </section>
<!--SCROLL SECTION ENDED-->

</template>

<script>
export default {
    name: "HeaderComponent"
}
</script>

<style lang="scss" scoped>

.cont{
    .menu-items{
        a{
            font-style: normal;
            color: #FFF;
            font-family: Inter,sans-serif;
            margin-right: 50px;
            font-size: 18px;
            font-weight: 500;
            line-height: 22px;
        }
    }
    .lines{
        width: 490px;
        height: 428px;
        top: 0;
        left: 0;
    }
    .eclipse{
        left:0;
        top: 200px;
        opacity: .4;
    }
    .eclipse-star{
    left: 55px;
    top: 250px;

    }
    .menu-star{
        top: 77px;
        right: 99px;
        min-width: 54px;
        min-height: 54px;
    }
}
#main{
    margin-top: 70px;
    .title{
        .digital{
            margin-left: 150px;
            .long-line{
                width: 717px;
                left: 595px;
                top: 10px;
            }
        }
        .agency{
            .right-image{
                top: 0;
                left:945px ;
                margin-left: 30px!important;
                z-index:1;
                .right-image-star{
                    top:85px;
                    left:480px;
                }
                .right-image-bottom-circle{
                    top: 375px;
                    left: 300px;
                    z-index: 99;
                     background: rgba(255, 255, 255, 0.5);
                    backdrop-filter: blur(25px);
                    border-radius: 50%;
                    opacity: 2;
                }
            }
        }
        h2{
            font-size: 150px;
            color: #FFFFFF;
            line-height: 181px;
        }
        .world-class{
            top: 70px;
            left: 300px;
            color: #FFFFFF;
            .rotate-text{
                left: 59px;
                transform: rotate(332deg);
            }
            .rotate-lines{
                top: -90px;
                left: -30px;
            }
        }
    }
    .explain{
        text-align: left;
        margin-right: auto;
        margin-left: auto;
        margin-top: 22px;
        width: 555px;
        height: 74px;
        .explain-text{
            font-family: Inter;
            font-style: normal;
            font-weight: 400;
            font-size: 24px;
            line-height: 40px;
            color:#E0E5F3 ;
            opacity: .8;
            margin-right:50px ;
        }
        .our-project{
            width: 200px;
            margin-top: 40px;
            .yellow-button{
                color: #0A142F;
                opacity: 1;
                padding: 20px 30px;
                border-radius: 30px;
                background-color: #FFC93E;
                height: 60px;
            }
            .left-image{
                top: 0px;
                right: 264px;
                z-index:2;
            }
            .eclipse{
                position: absolute;
                top: 190px;
                right: 190px;
                z-index: 1;
                opacity: .5;
            }
        }
    }
}

.scroll-down{
    top: 850px;
    left: 50%;
    .rotate-scroll{
        transform: rotate(270deg);
        color: #F3F5F6;
        font-size: 14px;
        font-weight: 400;
        line-height: 17px;

    }
    .scroll-img{
        width: 15px;
        height: 15px;
        margin-top: 40px;
    }
}
</style>