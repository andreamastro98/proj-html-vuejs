<script>
    export default{
        name:'NavComp'
    }
</script>

<template>
    <div>
        <div class="info-nav">
            <div class="container d-flex justify-content-between">
                <div>
                    <span>
                        <i class="fa-solid fa-clock mx-2"></i>Open Hours: Mon - Sat - 9:00 - 18:00
                    </span>
                </div>
                <div>
                    <span class="me-3">
                        <i class="fa-solid fa-phone"></i> +1(305) 1234-5678
                    </span>
                    <span class="mx-3">
                        <i class="fa-solid fa-envelope"></i> hello@example.com
                    </span>
                    <span class="mx-3">
                        <a href="https://www.facebook.com/"><i class="fa-brands fa-facebook-f"></i></a>
                    </span>
                    <span class="mx-3">
                        <a href="https://twitter.com/?lang=it"><i class="fa-brands fa-twitter"></i></a>
                    </span>
                    <span class="ms-3">
                        <a href="https://it.linkedin.com/"><i class="fa-brands fa-linkedin-in"></i></a>
                    </span>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>

.info-nav{
    padding: 0.9rem 0 0.9rem 0;
    background-color: #21333E;
    i,span{
        color: #C0C3D0;
    }
}

</style>