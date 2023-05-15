<script>
    export default{
        name: 'ExpertSingleCardComp',
        props: {
            singlecard: Object
        },
        data(){
            return{
                path:'../../public/img'
            }
        }
    }
</script>

<template>
    <div class="width my-3 d-flex align-items-center item">
        <img :src="path + singlecard.img" :alt="singlecard.name">
        <div class="mx-4">
            <h5>{{ singlecard.name }}</h5>
            <p class="my-3">{{ singlecard.job }}</p>
            <a href="https://www.facebook.com/"><i class="fa-brands round fa-facebook-f"></i></a>
            <a href="https://twitter.com/?lang=it"><i class="fa-brands round fa-twitter"></i></a>
            <a href="https://it.linkedin.com/"><i class="fa-brands round fa-linkedin-in"></i></a>
        </div>
    </div>
</template>

<style lang="scss" scoped>

.item{
    position: relative;
    bottom: 0;
    transition: bottom 0.5s;
    cursor: pointer;
    &:hover{
        bottom: 15px;
    }
}
.width{
    width: 45%;
}

img{
    width: 35%;
    border-radius: 6px;
}

h5{
    text-transform: uppercase;
    color: black;
    font-weight: bold;
}

p{
    color: #936D75;
    text-transform: uppercase;
    font-size: 15px;
}

</style>