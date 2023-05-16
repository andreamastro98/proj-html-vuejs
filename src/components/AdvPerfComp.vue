<script>
    export default{
        name:'AdvPerfComp'
    }
</script>

<template>
    <div class="container text-center">
        <h5 class="small-green-text">INTRODUCTION VIDEO</h5>

        <div class="my-4">
            <span>Advisory </span>
            <span class="green-text">Performance</span>
        </div>
        
        <p class="mb-5">Financial executives need to review their strategies, operating models and capabilities so that their <br> areas can generate sound information for better decision making.</p>

        <div id="img">
            <img src="../../public/img/video-1.jpg" alt="">
            <a href="#"><i class="fa-solid fa-play"></i></a>
        </div>
        
    </div>
</template>



<style lang="scss" scoped>

img{
    width: 70%;
    border-radius: 10px;
}

.container{
    padding: 7rem 0 7rem 0;
    span{
        font-weight: bold;
        font-size: 3.5rem;
    }
    p{
        color: #676669;
        font-size: 17px;
    }
}

i{
    position: relative;
    color: rgba(255,255,255,0.5);
    right: 36%;
    font-size: 50px;
    transform: translate( 0, 36% );
    transition: font-size 1s, color 1s;
    &:hover {
        font-size: 70px ;
        color: rgba(255,255,255,0.9)
    }
}

</style>