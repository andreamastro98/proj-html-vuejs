<script>
    import BusinessSingleCard from './BusinessSingleCardComp.vue'
    import { store } from '../store';


    export default{
        name:'BusinessAreaComp',
        components:{
            BusinessSingleCard,
        },
        data(){
            return{
                cards:[
                    {
                        icon: "fa-solid fa-network-wired",
                        title:"Audit & Assurance",
                        description:"Loren ipsum dolor sit amet consectetur adipiscing elit",
                    },
                    {
                        icon: "fa-solid fa-briefcase",
                        title: "Financial Advisory",
                        description: "Loren ipsum dolor sit amet consectetur adipiscing elit",
                    },
                    {
                        icon: "fa-solid fa-chart-simple",
                        title: "Analytics and M&A",
                        description: "Loren ipsum dolor sit amet consectetur adipiscing elit",
                    },
                    {
                        icon: "fa-solid fa-money-bill-trend-up",
                        title: "Middle Marketing",
                        description: "Loren ipsum dolor sit amet consectetur adipiscing elit",
                    },
                    {
                        icon: "fa-solid fa-gavel",
                        title: "Legal Consulting",
                        description: "Loren ipsum dolor sit amet consectetur adipiscing elit",
                    },
                    {
                        icon: "fa-solid fa-inbox",
                        title: "Regulatory Risk",
                        description: "Loren ipsum dolor sit amet consectetur adipiscing elit",
                    },
                ],

                store
            }
        },
    }
</script>


<template>
    <div class="bg">
        <div class="container-3">
            <span class="small-green-text">OUR BUSINESS AREA</span>
            <div class="my-3">            
                <span class="white">Excellence in </span>
                <span class="highlighted-text-2 white"> Services</span>            
            </div>
            <div class="d-flex justify-content-between mb-5">
                <p>We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowned professionals. These are some options that you can hire.</p>
                <button type="button" class="btn btn-2" @click="store.seeall = !store.seeall">SEE ALL</button>
            </div>
        
            <div class="d-flex flex-wrap justify-content-between">
                <BusinessSingleCard v-for="(elem, index) in cards"
                    :key="index"
                    :singlecard="elem">
                </BusinessSingleCard>

                <div v-if="store.seeall" class="card mb-5" style="width: 18rem;">
                  <div class="card-body">
                    <div class="d-flex justify-content-between mb-3">
                        <i class="fa-solid fa-truck-fast"></i>
                        <i class="fa-solid fa-arrow-right"></i>
                    </div>
                    <h5 class="card-title white-3 my-4">Lorem Ipsum</h5>
                    <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                  </div>
                </div>

                <div v-if="store.seeall" class="card mb-5" style="width: 18rem;">
                  <div class="card-body">
                    <div class="d-flex justify-content-between mb-3">
                        <i class="fa-solid fa-cloud"></i>
                        <i class="fa-solid fa-arrow-right"></i>
                    </div>
                    <h5 class="card-title white-3 my-4">Lorem Ipsum</h5>
                    <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                  </div>
                </div>

                <div v-if="store.seeall" class="card mb-5" style="width: 18rem;">
                  <div class="card-body">
                    <div class="d-flex justify-content-between mb-3">
                        <i class="fa-solid fa-wifi"></i>
                        <i class="fa-solid fa-arrow-right"></i>
                    </div>
                    <h5 class="card-title white-3 my-4">Lorem Ipsum</h5>
                    <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                  </div>
                </div>

            </div>
                
        </div>
    </div>
</template>



<style lang="scss" scoped>

p{
    color: #bcbdbd;
    font-size: 17px;
    width: 80%;
}

.card {
    --bs-card-spacer-y: 2.5rem;
    --bs-card-spacer-x: 2.5rem;
    --bs-card-bg: #19191F;
}

.bg{
    background-color: #111117;
}

.card{
    width: 30%!important;
    position: relative;
    bottom: 0;
    transition: bottom 0.5s;
    cursor: pointer;
    &:hover{
        bottom: 20px;
    }
}

div i:first-child{
    color: #098081;
    font-size: 40px;
}

div i:last-child{
    font-size: 25px;
    color: #098081;
    filter: brightness(0.5);
}


</style>