<template>
<div class="container">
    <div class="help-section flex justify-around items-center container">
        <h3 class="title">Service We Can Help You</h3>
        <button @mouseover="hover=true" @mouseleave="hover = false" class="button flex items-center ">See All
            <img v-if="hover" style="width: 15px; height: 15px" class="ml-2.5" src="../image/turn.svg" alt="">
            <img v-else style="width: 15px; height: 15px" class="ml-2.5" src="../image/turn-white-icon.svg" alt="">
        </button>
    </div>
    <div  class="card-conteiner container items-center justify-around grid grid-cols-2 grid-rows-2 text-white ">
        <div v-for="(item,index) in items" :key="index" class="card">
            <img :src="items[index].image_url" alt="">
            <div class="title">{{ items[index].title }}</div>
            <div class="paragraph">{{ items[index].paragraph }}</div>
        </div>


    </div>
</div>
</template>

<script>
export default {
    name: "ServicePage",
    data(){
        return{
            hover:false,
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
    .button{
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



.card-container{
    .card{
        .title{
            font-style: normal;
            font-weight: 600;
            font-size: 30px;
            line-height: 36px;
            color: yellow;
            padding: 100px;
        }
        .paragraph{
            font-family: 'Inter';
            font-style: normal;
            font-weight: 400;
            font-size: 16px;
            line-height: 30px;
            /* or 188% */


            color: #E0E5F3;
        }
    }
}

</style>