<script>

    import NewsSingleCardComp from './NewsSingleCardComp.vue'

    export default{
        name:'NewsComp',
        components:{
            NewsSingleCardComp,
        },
        data(){
            return{
                card:[
                    {
                        img:'/news-1.jpg',
                        title:'Increasing creativity is possible for everyone'
                    },
                    {
                        img: '/news-2.jpg',
                        title: 'Because market reasearch is part of the business plan'
                    },
                    {
                        img: '/news-3.jpg',
                        title: 'Working from home is now a trend'
                    },
                ]
            }
        }
    }
</script>


<template>
    <div class="bg">
        <div class="container-3">
            <span class="small-green-text">our editorial content</span>
            <div class="my-4">
                <span class="span-title">Latest </span>
                <span class="green-text span-title">News</span>
            </div>
            <div class="d-flex justify-content-between mb-5 align-items-center">
                <p>Every week we publish content about what is best in the business world.</p>
                <button type="button" class="btn btn-1">SEE ALL</button>
            </div>
            <div class="d-flex justify-content-between">
                <NewsSingleCardComp v-for="( elem, index) in card"
                :key="index"
                :singlecard="elem">
                </NewsSingleCardComp>
            </div>
        </div>
    </div>
        
</template>


<style lang="scss" scoped>

.bg{
    background-color: #EEF4ED;
}

p{
    color: #676669;
    font-size: 17px;
}

</style>