<template>
    <div class="container flex flex-col justify-center items-center ">
        <h4 class="title mb-8 ">Our Latest Projects</h4>
        <div class="menu flex justify-center">
            <div class="menu-item cursor-pointer">All</div>
            <div class="menu-item cursor-pointer">UI/UX</div>
            <div class="menu-item cursor-pointer">Web Design</div>
            <div class="menu-item cursor-pointer">Branding</div>
            <div class="menu-item cursor-pointer">Interaction</div>
        </div>
        <div class="row flex mt-10 justify-center ">
            <div style="max-width: 564px" class="left-col flex flex-col justify-center mx-5">
                <img style="width: 554px;height: 500px;" src="../image/latest-left.png" alt="">
                <div class="row-title">
                    Talent.com - Logo, Full Redesign and Branding
                </div>
                <div class="row-paragraph">
                    Talent.com a new brand identity using their core values of optimism, transparency and approachability as inspiration. As a result, we were
                    able to create the most streamlined
                </div>
            </div>
            <div  style="max-width: 564px" class="right-col justify-center mx-5">
                <img  style="max-width: 554px;height: 500px;" src="../image/latest-right.png" alt="">
                <div class="row-title">
                    Bonfire - Landing Page Design Webby Awards Nomination
                </div>
                <div class="row-paragraph">
                    Pretty excited to announce that we just got nominated at the Webby Awards! easy to understand and to use should be essential for every business owner who uses their website.
                </div>
            </div>
        </div>
        <button class="button flex items-center ">Load More
            <img style="width: 15px; height: 15px" class="ml-2.5" src="../image/turn-white-icon.svg" alt="">
        </button>
    </div>
</template>

<script>
export default {
    name: "LatestProjects"
}
</script>

<style lang="scss" scoped>
.container{
    margin-top: 120px;
    .title{
        color: #FFFFFF;
        font-size: 48px;
        line-height: 60px;
        font-weight: 700;
    }
    .menu{
        transition: .5s;
        margin-left: 20px;
        .menu-item{
            margin-right: 50px;
            color: #FFFFFF;
        }
        .menu-item:hover{
            color: #FFC93E;
        }
    }
    .row{
        text-align: left;

        .row-title{
            margin-left: 10px;
            margin-top: 32px;
            font-weight: 700;
            color: #FFFFFF;
            font-size: 24px;
            line-height: 36px;
            max-width: 393px;
        }
        .row-paragraph{
            margin-left: 10px;
            margin-top: 32px;
            color: #E0E5F3;
            font-size: 16px;
            font-width: 400;
            line-height: 30px;
        }
    }
    .button{
        display: flex;
        align-items: center;
        justify-content: center;
        color: #FFFFFF;
        opacity: 1;
        padding: 20px;
        border-radius: 30px;
        border: 1px solid;
        height: 60px;
        margin-top: 48px;
        transition: .3s;
        width: 200px!important;
    }
    .button:hover{
        color: #0A142F;
        opacity: 1;
        border-radius: 30px;
        background-color: #FFC93E;
        height: 60px;
        svg{
            fill: #0A142F;
        }
    }
}
</style>