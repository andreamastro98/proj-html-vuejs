<script>
    export default{
        name:'ResultsComp'
    }
</script>

<template>
    <div class="bg">
        <div class="container-2 text-center">
            <h5 class="small-green-text mb-5">WHAT ARE WE DOING</h5>
            <div class="mb-5">
                <span class="highlighted-text-2 white">Results</span>
                <span class="white"> in Numbers</span>
            </div>
            <div class="d-flex justify-content-between mt-5">
                <div>
                    <p class="green">128</p>
                    <span class="white-2">Certifications</span>
                </div>
                <div>
                    <p class="green">230</p>
                    <span class="white-2">Employees</span>
                </div>
                <div>
                    <p class="green">517</p>
                    <span class="white-2">Customers</span>
                </div>
                <div>
                    <p class="green">94</p>
                    <span class="white-2">Countries Served</span>
                </div>
            </div>        
        </div>
    </div>
        
</template>


<style lang="scss" scoped>

.bg{
    background-image: url(../../public/img/adrian-schwarz-XS7q-baZrmE-unsplash.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
}

.green{
    font-weight: bold;
    font-size: 3rem;
    color: #098081;
}

</style>