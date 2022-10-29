<template>
<div class="container">
    <div class="help-section flex justify-around items-center container">
        <h3 class="title">Service We Can Help You</h3>
        <button class="button flex items-center ">Read More
            <TurnWhite class="ml-2 arrow-white"></TurnWhite>
        </button>
    </div>
    <section class="card-section">
        <div  class="card-container container2 flex items-center grid-cols-2 justify-center text-white ">
            <div style="border-radius: 50px 0px 0px 0px; " class="card mx-4 ">
                <div class="card-content">
                    <img src="../image/write-icon.svg" alt="">
                    <h3 class="card-title">{{items[1].title}}</h3>
                    <div class="p paragraph">
                        {{items[1].paragraph}}
                    </div>
                    <button class="button flex items-center ">Read More
                        <TurnWhite class="ml-2 arrow-white"></TurnWhite>
                    </button>
                </div>
            </div>
            <div style="border-radius: 0px 50px 0px 0px; "  class="card mx-4 mt-20 ">
                <div class="card-content">
                    <img src="../image/docs-icon.svg" alt="">
                    <h3 class="card-title">{{items[2].title}}</h3>
                    <div class="p paragraph">
                        {{items[2].paragraph}}
                    </div>
                    <button class="button flex items-center ">Read More
                        <TurnWhite class="ml-2"></TurnWhite>
                    </button>
                </div>
            </div>

        </div>
        <div  class="card-container container2 flex items-center grid-cols-2 justify-center text-white ">
            <div style="border-radius: 0px 0px 0px 50px; " class="card mx-4 ">
                <div class="card-content">
                    <img src="../image/write-icon.svg" alt="">
                    <h3 class="card-title">{{items[1].title}}</h3>
                    <div class="p paragraph">
                        {{items[1].paragraph}}
                    </div>
                    <button class="button flex items-center ">Read More
                        <TurnWhite class="ml-2"></TurnWhite>
                    </button>
                </div>
            </div>
            <div style="border-radius: 0px 0px 50px 0px; "  class="card mx-4 mt-20  ">
                <div class="card-content">
                    <img src="../image/docs-icon.svg" alt="">
                    <h3 class="card-title">{{items[2].title}}</h3>
                    <div class="p paragraph">
                        {{items[2].paragraph}}
                    </div>
                    <button class="button flex items-center ">Read More
                        <TurnWhite class="ml-2"></TurnWhite>
                    </button>
                </div>
            </div>


        </div>
    </section>

</div>
</template>

<script>
import TurnWhite from "@/components/TurnWhite";
export default {
    name: "ServicePage",
    components:{
        TurnWhite,
    },
    data(){
        return{
            hover:false,
            hover_content:false,
            items:[
                {
                    image_url:`../image/geo-icon.svg`,
                    title : 'Branding',
                    paragraph: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. A consequat nunc id purus pretium sagittis diam quis massa. Nulla ridiculus nullam bibendum luctus viverra. Eu pellentesque sem sed platea diam dignissim duis purus.  '
                },
                {
                    image_url:'../image/write-icon.svg',
                    title : 'Content Writing',
                    paragraph: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. A consequat nunc id purus pretium sagittis. Nulla ridiculus nullam bibendum luctus viverra. Eu pellentesque sem sed platea diam dignissim duis purus. '

                }
                ,
                {
                    image_url:'../image/docs-icon.svg',
                    title : 'UX Research',
                    paragraph: ' Lorem ipsum dolor sit amet, consectetur adipiscing elit. A consequat nunc id purus pretium sagittis diam quis massa. Nulla ridiculus nullam bibendum luctus viverra. Eu pellentesque sem sed platea diam dignissim duis purus. '
                },
                {
                    image_url:'../image/tv-icon.svg',
                    title : 'Web Design',
                    paragraph: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. A consequat nunc id purus pretium sagittis diam quis massa. Nulla ridiculus nullam bibendum luctus viverra. Pellentesque sem sed platea diam dignissim duis purus.  '
                }
            ]

        }
    },
    methods: {
        consol(){
            console.log(this.items)
        }
    },

}
</script>

<style lang="scss" scoped>
*{
    font-family: inter;
}

.container{
    margin-top: 120px;
}
.help-section{
    .title{
        text-align: left;
        color: #FFFFFF;
        width: 382px;
        height: 116px;
        font-weight: 700;
        font-size: 48px;
        line-height: 58px;
        text-transform: capitalize;
    }
}
.button{
    .arrow-white{
    }
    color: #FFFFFF;
    opacity: 1;
    padding: 20px;
    border-radius: 30px;
    border: 1px solid;
    height: 60px;
    margin-top: 48px;
    transition: .3s;
}
.button:hover{
    .arrow-white div{
        fill: #0A142F !important;
    }
    color: #0A142F;
    opacity: 1;
    border-radius: 30px;
    background-color: #FFC93E;
    height: 60px;
}


.card-section{
    .container2:nth-child(2){
        margin-top: -50px;
    }
    .card-container{
        .card{
            background: #353F5B;
            width: 555px;
            padding: 34px 83px 44px 83px;
            text-align: left;
            .card-content {
                .card-title {
                    margin-top: 23px;
                    margin-bottom: 24px;
                    font-style: normal;
                    font-weight: 600;
                    font-size: 30px;
                    line-height: 36px;
                    color: #fff;
                }

                .paragraph {
                    font-style: normal;
                    font-weight: 400;
                    font-size: 16px;
                    line-height: 30px;

                    color: #E0E5F3;

                    color: #E0E5F3;
                }

                .button {
                    color: #FFFFFF;
                    opacity: 1;
                    padding: 20px;
                    border-radius: 30px;
                    border: 1px solid;
                    height: 60px;
                    margin-top: 48px;
                    transition: .3s;
                }

                .button:hover {
                    color: #0A142F;
                    opacity: 1;
                    border-radius: 30px;
                    background-color: #FFC93E;
                    height: 60px;
                    .turn-white > svg{
                        fill: #0A142F !important;
                    }
                }
            }
        }
    }
}

</style>