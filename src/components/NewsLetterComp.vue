<script>
    export default{
        name:'NewsLetterComp'
    }
</script>

<template>
    <div class="bg">
        <div class="container-4 d-flex justify-content-between">
            <div class="width-45">
                <span class="small-green-text">newsletter</span>
                <div class="my-3">            
                    <span class="highlighted-text-2 white">Know</span>
                    <span class="white"> First</span>                                
                </div>
                <p>Follow closely and receivecontent aboutour company and the news of the current market.</p>
            </div>
            <div class="width-45">
                <input class="form-control form-control-lg mt-3 mb-4" type="text" placeholder="name" aria-label=".form-control-lg example">

                <input class="form-control form-control-lg mb-4" type="email" placeholder="email" aria-label=".form-control-lg example">

                <button type="button" class="btn btn-1">SUBSCRIBE</button>
            </div>
        </div>
    </div>
</template>



<style lang="scss" scoped>

.bg{
    background-color: #111117;
}

.container-4{
    padding: 7rem 0 7rem 0;
    width: 50%;
    margin: 0 auto;
}

.width{
    width: 45%;
}

p{
    color: #bcbdbd;
    font-size: 17px;
}

.form-control{
    background-color: #1D1D23;
    border: #1D1D23;
}

.form-control::placeholder{
    color: #bcbdbd91;
}
</style>
