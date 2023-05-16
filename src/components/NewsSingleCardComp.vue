<script>
    export default{
        name:'NewsSingleCardComp',
        props: {
        singlecard: Object
        },
    data() {
        return {
            path: '../../public/img'
        }
    }
    }
</script>

<template>
    <div class="col-4">
        <img :src="path + singlecard.img" :alt="singlecard.img">
        <p>{{ singlecard.title }}</p>
    </div>
</template>



<style lang="scss" scoped>

div{
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

p{
    position: relative;
    color: #F9F9F9;
    bottom: 9rem;
    margin: 2rem;
    font-size: 23px;
    font-weight: bold;
}

</style>