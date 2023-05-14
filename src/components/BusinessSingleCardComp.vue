<script>
    export default{
        name:'BusinessSingleCard',
        props:{
            singlecard: Object
        },
    }
</script>

<template>
    <div class="card mb-5" style="width: 18rem;">
      <div class="card-body">
        <div class="d-flex justify-content-between mb-3">
            <i :class="singlecard.icon"></i>
            <i class="fa-solid fa-arrow-right"></i>
        </div>
        <h5 class="card-title white-3 my-4">{{ singlecard.title }}</h5>
        <p class="card-text">{{ singlecard.description }}</p>
      </div>
    </div>
</template>



<style lang="scss" scoped>

.card{
    width: 30%!important;
}

p{
    color: #bcbdbd;
    font-size: 17px;
    width: 80%;
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