<script>
    import BusinessSingleCard from './BusinessSingleCardComp.vue'


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
                ]
            }
        }
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
                <button type="button" class="btn btn-2">SEE ALL</button>
            </div>
        
            <div class="d-flex flex-wrap justify-content-between">
                <BusinessSingleCard v-for="(elem, index) in cards"
                    :key="index"
                    :singlecard="elem">
                </BusinessSingleCard>
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


</style>