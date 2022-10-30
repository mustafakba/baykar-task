<template>
<div class="title flex text-left ml-44">Categories</div>
    <div class="ml-40 mr-20">
        <Splide  :options="{ rewind: true }" data-splide='{"type":"loop","perPage":4, "gap":60}' aria-label="My Favorite Images" >
            <SplideSlide v-for="(item,index) in items" :key="index" class="">
               <div class="card">
                   <img :src="item.image_url" alt="">
                   <div class="type mt-14">
                       <span>{{items[index].type}}</span>
                   </div>
               </div>
            </SplideSlide>
        </Splide>
    </div>
    <div class="ml-40 mr-20 mt-20">
        <Splide  :options="{ rewind: true }" data-splide='{"type":"loop","perPage":4, "gap":60}' aria-label="My Favorite Images" >
            <SplideSlide v-for="(item,index) in items" :key="index" class="">
                <div class="card">
                    <img :src='item.image_url' alt="">
                    <div class="type mt-14">
                        <span>{{items[index].type}}</span>
                    </div>
                </div>
            </SplideSlide>
        </Splide>
    </div>


</template>

<script>
import {  Splide,SplideSlide } from '@splidejs/vue-splide'
import CategoriesImage from '@/image/categories.png'
import CategoriesImage2 from '@/image/categories-img-2.png'
import CategoriesImage3 from '@/image/categories-img-3.png'
import CategoriesImage4 from '@/image/categories-img-4.png'
export default {

    name: "CategoriesPage",
    components:{
        Splide,
        SplideSlide
    },
    data(){
        return{
            items:[
                {
                    image_url:CategoriesImage,
                    type:'Games'
                },
                {
                    image_url:CategoriesImage2,
                    type: 'Sports'
                },
                {
                    image_url:CategoriesImage3,
                    type:'Metaverse'
                },
                {
                    image_url:CategoriesImage4,
                    type: 'Art'
                }

            ]
        }
    }
}
</script>

<style scoped>
.title{
    margin-top: 120px;
    margin-bottom: 50px;
    font-family: 'Inter';
    font-style: normal;
    font-weight: 700;
    font-size: 48px;
    line-height: 58px;
    /* identical to box height */
    text-align: center;
    text-transform: capitalize;

    color: #FFFFFF;
}
.container{
    max-width: 1470px;
    display: flex;
    justify-content: center;
}
.card{
    padding: 10px 10px 10px 10px;
    max-width: 245px;
    height: 367px;
    border-radius: 50px;
    background: #3A425A;
    font-style: normal;
    font-weight: 700;
    font-size: 20px;
    line-height: 30px;
    /* identical to box height */

    text-align: center;
    letter-spacing: 0.04em;

    color: #FFFFFF;
}
</style>