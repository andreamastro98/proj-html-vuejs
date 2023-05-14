<script>
    import ExpertSingleCardComp from './ExpertSingleCardComp.vue'

    export default{
        name:'ExpertComp',
        components:{
            ExpertSingleCardComp
        },
        data() {
            return {
                cards: [
                    {
                        img: "/team-1.jpg",
                        name: "David Cooper",
                        job: "cto & co-founder",
                    },
                    {
                        img: "/team-3.jpg",
                        name: "Oliver Jones",
                        job: "chief procurement",
                    },
                    {
                        img: "/team-2.jpg",
                        name: "Emma Lopez",
                        job: "chief marketing",
                    },
                    {
                        img: "/team-4.jpg",
                        name: "T. Johnson",
                        job: "ceo & president",
                    },
                ]
            }
        }
    }
</script>

<template>
    <div class="container-3">
        <span class="small-green-text">we like what we do</span>
        <div class="d-flex justify-content-between">
            <div class="first-col">
                <div class="my-4">            
                    <span class="green-text span-title">Team</span>
                    <span class="span-title"> of Experts</span>
                </div>
                <p class="grey">Ethics and integrity are the bases on which our professionals build their careers. They are fundamentals that become daily attitudes</p>

                <div class="d-flex justify-content-between flex-wrap">
                    <ExpertSingleCardComp v-for="( elem, index) in cards"
                    :key="index"
                    :singlecard="elem"></ExpertSingleCardComp>
                </div>
                
            </div>

            <div class="green-box">
                <p class="name">President Speech</p>

                <p class="grey-2">Loren ipsum dolor sit amet, consectetur adipiscing elit. Praesent ut lacinia diam. <br><br> Vivamus efficitur et est quis posuere. Nulla sollicitudin vulputate dui, id pretium tortor congue eu Integer aliquet justo eu quam volutpat ullamcorper. <br><br> Duis ut hendrerit mauris. Phasellus faucibus ut enim vel tincidunt. Nunc venenatis a dui et laoreet.</p>
                <div class="d-flex justify-content-between">
                    <p class="grey-3">T. Johnson</p>
                    <i class="fa-solid fa-quote-right"></i>
                </div>                
            </div>
        </div>
        
    </div>
</template>



<style lang="scss" scoped>

.grey{
    color: #676669;
    font-size: 17px;
}

.first-col{
    width: 65%;
}

.green-box{
    padding: 2rem;
    background-color: #048383;
    border-radius: 6px;
    width: 30%;
    margin-top: 2rem;
}

.name{
    color: white;
    font-weight: bold;
    font-size: 25px;
}

.grey-2{
    font-size: 17px;
    color: #BDD9D9;
    font-weight: 400;
}

.grey-3{
    font-size: 18px;
    color: #BDD9D9;
    font-weight: bold;
}

i{
    color: #046162;
    font-size: 2rem;
}

</style>