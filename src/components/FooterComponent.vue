<template>

   <div class="container relative">
        <EclipseSvg class="absolute eclipse"></EclipseSvg>
       <div class=" flex grid  grid-flow-col gap-2">
           <div class="grid-flow-col flex ml-20">
               <div class="card relative">
                   <img class="dots absolute top-0 left-0" src="../image/dots.svg" alt="">
                   <h6 class="title">Sign Up to Receive Product Updates and More</h6>
                   <div class="mail flex justify-between">
                       <span>youremail@gmail.com</span>
                       <img src="../image/right-arrow.svg" alt="">
                   </div>
                   <hr>
               </div>
           </div>
           <div class="contact-area grid-flow-col flex justify-center items-center">
               <div class="office mr-28">
                   <h6>Office</h6>
                   <p>545, Street 11, Block F
                       California, U.S.A</p>
               </div>
               <div class="contact">
                   <h6>Contact</h6>
                   <p>+90 302 300 3215</p>
                   <p>ouraddress@email.com</p>
               </div>
           </div>
       </div>
       <div class="footer-bottom flex justify-between items-center my-12">
           <div class="all-right-reserved">
               <span>2022. All Rights Reserved</span>
           </div>
           <div class="privacy">
               <span>Terms & Conditions <span class="ml-5">Privacy</span>     </span>
           </div>
           <div class="social flex ">
               <TwitterIcon class="ease-in-out duration-300 mr-7 cursor-pointer hover"></TwitterIcon>
               <FacebookIcon class="ease-in-out duration-300 mr-7 cursor-pointer hover"></FacebookIcon>
               <BallIcon class="ease-in-out duration-300 mr-7 cursor-pointer hover" ></BallIcon>
               <GithubIcon class="ease-in-out duration-300 mr-7 cursor-pointer hover"></GithubIcon>
           </div>
       </div>

   </div>

</template>

<script>
import EclipseSvg from "@/components/Icons/EclipseSvg";
import TwitterIcon from "@/components/Icons/TwitterIcon";
import FacebookIcon from "@/components/Icons/FacebookIcon";
import BallIcon from "@/components/Icons/BallIcon";
import GithubIcon from "@/components/Icons/GithubIcon";
export default {
    name: "FooterComponent",

    components:{
        TwitterIcon,
        FacebookIcon,
        BallIcon,
        GithubIcon,
        EclipseSvg

    }
}
</script>

<style lang="scss" scoped>
*{
    overflow-x: hidden;
;
}
.container{
    z-index: 2;
    margin-top: 105px;
    background: #3B435A;
    width: 100%;
    height: 100%;
    padding: 80px 50px 10px 80px;
    .eclipse{
        overflow: hidden;
        margin-top: -150px;
        right: -50px;
        z-index: 1;
        opacity: 1;
    }
}
.card{
    .dots{
        top: -45px;
        left: -15px;
        transform: rotate(90deg);
    }
    text-align: left;
    width: 624px;
    padding: 80px 50px;
    background: #FFC93E;
    border-radius: 30px;
    hr{
        border-top: .5px solid #0A142F;
        margin-top: 15px;
        background-color: #0A142F;
        color: #0A142F;
    }
    .title{
        margin-bottom: 15px;
        max-width: 528px;
        font-style: normal;
        font-weight: 600;
        font-size: 20px;
        line-height: 150%;
        color: #0A142F;
    }
    .mail{
        color: #0A142F;

    }
}
.contact-area{
    text-align: left;
    h6{
        font-style: normal;
        font-weight: 600;
        font-size: 18px;
        line-height: 18px;
        color: #FFFFFF;
        margin-bottom: 16px;

    }
    p{
        max-width: 257.5px;
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 30px;
        color: #FFFFFF;
    }
}
.footer-bottom{
    color: #E0E5F3;
}
.hover:hover{
    color: #FFC93E;
}


</style>