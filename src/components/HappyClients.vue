<template>
    <h2 class="title">What Say Happy Clients</h2>
    <Splide  style="margin-left: 180px" data-splide='{"type":"loop","perPage":2, "gap":350, "arrowPath":"M37.8 28.0004C37.8 28.186 37.7262 28.3641 37.595 28.4954C37.4637 28.6266 37.2857 28.7004 37.1 28.7004L20.5898 28.7004L24.9956 33.1048C25.127 33.2362 25.2009 33.4145 25.2009 33.6004C25.2009 33.7863 25.127 33.9645 24.9956 34.096C24.8642 34.2274 24.6859 34.3013 24.5 34.3013C24.3141 34.3013 24.1358 34.2274 24.0044 34.096L18.4044 28.496C18.3392 28.431 18.2875 28.3537 18.2522 28.2687C18.2169 28.1836 18.1987 28.0925 18.1987 28.0004C18.1987 27.9083 18.2169 27.8171 18.2522 27.7321C18.2875 27.6471 18.3392 27.5698 18.4044 27.5048L24.0044 21.9048C24.1358 21.7733 24.3141 21.6995 24.5 21.6995C24.6859 21.6995 24.8642 21.7733 24.9956 21.9048C25.127 22.0362 25.2009 22.2145 25.2009 22.4004C25.2009 22.5863 25.127 22.7645 24.9956 22.896L20.5898 27.3004L37.1 27.3004C37.2857 27.3004 37.4637 27.3741 37.595 27.5054C37.7262 27.6367 37.8 27.8147 37.8 28.0004Z" }' :options="{ rewind: true }" aria-label="My Favorite Images">

        <div class="splidearrows">
            <button class="splidearrow splidearrow--next">Prev</button>
            <button class="splidearrow splide__arrow--prev">Next</button>
        </div>
        <SplideSlide v-for="(item,index) in commits " :key="index">
            <div class="card">
                <div class="content">
                    <img class="quotes" src="../image/quotes.svg" alt="">
                    <p style="line-height: 30px" class="my-8 content-text text-left">{{item.commit}} </p>
                    <div class="information flex justify-between items-center">
                       <div class="person flex">
                           <img src="../image/person-1.svg" alt="">
                           <div class="person-information  flex items-center flex-col justify-center ml-5">
                               <h5>{{item.person.fullName}}</h5>
                               <h6 class="job text-left">{{item.person.title}}</h6>
                           </div>
                       </div>
                        <div class="flex personal-rating">
                            <img style="width: 15px;height: 15px; margin-right: 8px;" v-for="(item,index) in 5" :key="index"  src="../image/bi_star-fill.svg" alt="">
                        </div>
                    </div>
                </div>

            </div>
        </SplideSlide>
    </Splide>
</template>

<script>
import {  Splide,SplideSlide } from '@splidejs/vue-splide';

export default {
    name: "HappyClients",
    components:{
        SplideSlide,
        Splide,

    },
    data(){
        return{
            commits:[
                {
                    person:{
                        image_url:'../image/person-1.svg',
                        fullName:'Brooklyn Simmons',
                        title:'Pendron.Inc,CEO',
                    },
                    commit:'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sit semper consequat in dolor mattis pellentesque suspendisse vulputate nec. Scelerisque elementum, consequat pharetra lectus eget vivamus ut. Magna aliquam tellus at volutpat cras aliquet facilisi quis adipiscing. Proin egestas et pellentesque augue pretium, amet. Natoque blandit augue integer maecenas mattis amet, nec.',
                    rating : 5
                },
                {
                    person:{
                        image_url:'../image/person-1.svg',
                        fullName:'Jenny Wilson',
                        title:'Battero.Inc,CEO',
                    },
                    commit:'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sit semper consequat in dolor mattis pellentesque suspendisse vulputate nec. Scelerisque elementum, consequat pharetra lectus eget vivamus ut. Magna aliquam tellus at volutpat cras aliquet facilisi quis adipiscing. Proin egestas et pellentesque augue pretium, amet. Natoque blandit augue integer maecenas mattis amet, nec.',
                    rating : 5
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

.title{
    display: flex;
    justify-content: start;
    margin-left: 180px;
    margin-top: 120px;
    margin-bottom: 40px;
    font-style: normal;
    font-weight: 700;
    font-size: 48px;
    line-height: 58px;
    /* identical to box height */

    text-align: center;
    text-transform: capitalize;

    color: #FFFFFF;
}
.card{
    border-radius: 50px;
    color: #E0E5F3;
    width: 750px;
    height: 439px;
    background-color: #353F5B;
    padding: 65px 53px 65px 80px;
    .content{
        .quotes{
            color: #F3F5F6;
            opacity: .3;
        }
        .content-text{
            color: #E0E5F3;
        }
    }
}
.job{
    align-self: flex-start;
    font-size: 14px;
    color: #FFC93E;
}
</style>