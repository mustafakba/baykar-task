<template>
    <h3 class="title text-left ml-44">Blog from insights</h3>
    <div class="container flex grid-rows-1 justify-center">
            <div v-for="(item,index) in items" :key="index" class="card flex flex-col self-start justify-center mx-8">
                <div class="card-image">
                    <img src="../image/blog-image-1.png" alt="">
                </div>
                <div class="type flex mt-6">
                    <span> {{items[index].type}} </span>
                </div>
                <div class="name-date flex mt-2.5 mb-2">
                    <span class="name">{{items[index].full_name}} {{items[0].date}}</span>
                </div>
                <div class="paragraph flex">
                    <p>{{items[index].paragraph}}</p>
                </div>
                <span><DefaultButton title="Read More"></DefaultButton></span>
            </div>

    </div>
</template>

<script>
import DefaultButton from "@/components/DefaultButton";
export default {
    name: "BlogFrom",
    components:{
        DefaultButton
    },
    data(){
        return{
            items:[
                {
                    image_url:'../image/blog-image-1.png',
                    type :'TECHNOLOGY',
                    full_name :'John Doe • ',
                    date :'19 Jan 2022',
                    paragraph :'A small business is only as good as its tools and it is totally true.',

                },
                {
                    image_url:"../image/blog-image-2.png",
                    type :'WEBINER',
                    full_name :'John Doe •',
                    date :' 19 Jan 2022',
                    paragraph :'Colaboration with team members that will be grow to business.',
                }


            ]

        }
    },
}
</script>

<style scoped>
.title{
    margin-bottom: 40px;
    margin-top: 120px;
    font-family: 'Inter';
    font-style: normal;
    font-weight: 700;
    font-size: 48px;
    line-height: 58px;
    /* identical to box height */

    text-transform: capitalize;

    color: #FFFFFF;
}
.type span{
    font-style: normal;
    font-weight: 500;
    font-size: 12px;
    line-height: 18px;
    /* identical to box height, or 150% */

    text-align: center;

    color: #0C1430;
    padding: 5px 12px;
    background: #F3F5F6;
    box-shadow: 0px 1px 2px rgba(105, 81, 255, 0.05);
    border-radius: 10px;
}
.name-date{
    opacity: .9;
    font-family: 'Inter';
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 24px;
    color: #FFFFFF;
}
.paragraph p{
    text-align: left;
    line-height: 38px;
    max-width: 554px;
    font-family: 'Inter';
    font-style: normal;
    font-weight: 700;
    font-size: 30px;
    line-height: 38px;

    color: #FFFFFF;

}
</style>