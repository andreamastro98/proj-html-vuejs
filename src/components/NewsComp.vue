<script>

    import NewsSingleCardComp from './NewsSingleCardComp.vue'
    import { store } from '../store';

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
                ],

                store
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
                <button type="button" class="btn btn-1" @click="store.seeall2 = !store.seeall2">SEE ALL</button>
            </div>
            <div class="d-flex row flex-wrap">
                <NewsSingleCardComp v-for="( elem, index) in card"
                :key="index"
                :singlecard="elem">
                </NewsSingleCardComp>

                <div v-if="store.seeall2" class="div col-4">
                    <img src="../../public/img/news-4.jpg" alt="news-4">
                    <p class="p">Tips for having a good relationship at work</p>
                </div>

                <div v-if="store.seeall2" class="div col-4">
                    <img src="../../public/img/news-5.jpg" alt="news-5">
                    <p class="p">David Cooper tells about the new opening in Baltimore</p>
                </div>
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

.div{
    width: 31%;
    text-align: center;
    margin-bottom: -5rem;
    opacity: 1;
    transition: opacity 1s ease 0s;
    cursor: pointer;
    &:hover{
        opacity: 0.6;
    }
}

img{
    width: 100%;
    border-radius: 6px;
    filter: brightness(0.5);
}

.p{
    position: relative;
    color: #F9F9F9;
    bottom: 9rem;
    margin: 2rem;
    font-size: 23px;
    font-weight: bold;
}

</style>