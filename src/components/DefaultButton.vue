<template>
    <button class="button flex items-center ">{{ title }}
        <ArrowIcon class="ml-2 arrow-white"></ArrowIcon>
    </button>
</template>

<script>
import ArrowIcon from "@/components/ArrowIcon";
export default {
    name: "DefaultButton",
    components:{
        ArrowIcon
    },
    props:{
        title:String
    }
}
</script>

<style scoped>
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
}
.arrow-white > svg {
    fill: #0A142F !important;

}


</style>