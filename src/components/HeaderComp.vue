<script>
    export default{
        name:'HeaderComp'
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


        <div id="carouselExampleIndicators" class="carousel slide">
            <div class="carousel-indicators">
                <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active"       aria-current="true" aria-label="Slide 1"></button>
                <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"      aria-label="Slide 2"></button>
                <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2"      aria-label="Slide 3"></button>
            </div>
            <div class="carousel-inner">
                <div class="carousel-item active">
                    <img src="../../img/bg-2.jpg" class="d-block w-100" alt="...">
                </div>
                <div class="carousel-item">
                    <img src="../../img/bg-1.jpg" class="d-block w-100" alt="...">
                </div>
                <div class="carousel-item">
                    <img src="../../img/bg-3.jpg" class="d-block w-100" alt="...">
                </div>
            </div>
            <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators"        data-bs-slide="prev">
              <span class="carousel-control-prev-icon" aria-hidden="true"></span>
              <span class="visually-hidden">Previous</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators"        data-bs-slide="next">
              <span class="carousel-control-next-icon" aria-hidden="true"></span>
              <span class="visually-hidden">Next</span>
            </button>
        </div>
        

        <nav class="navbar navbar-expand-lg">
            <div class="container d-flex align-items-center">
                <a class="navbar-brand" href="#">
                    <span class="logo-1">N E X </span>
                    <span class="logo-2">G E N</span>  
                </a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarNav">
                    <ul class="navbar-nav ms-auto d-flex align-items-center">
                        <li class="nav-item">
                            <a class="nav-link" aria-current="page" href="#">Home</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">About</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Services</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Team</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Blog</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#"><i class="fa-regular fa-user"></i></a>
                        </li>
                        <li class="nav-item">
                            <button type="button" class="btn btn-1">GET IN TOUCH</button>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>

        <div class="jumbo-text">
            <h1>Financial Risk</h1>
            <p class="my-4">The right outcomes depend on continuous rigor in governance, models, and processes across the finance function.</p>
            <button type="button" class="btn btn-1 me-2">GET IN TOUCH</button>
            <button type="button" class="btn btn-2 ms-2">READ MORE</button>
        </div>
        
    </div>
</template>

<style lang="scss" scoped>


.carousel{
    position: absolute;
    filter: brightness(0.6);
}
.info-nav{
    padding: 0.9rem 0 0.9rem 0;
    background-color: #21333E;
    i,span{
        color: #C0C3D0;
    }
}

.bg-jumbo{
    height: 110vh;
    width: 100vw;
    position: absolute;
    filter: brightness(70%);
}

.btn-1{
    background-color: #098081;
    color: #e7eee9;
    font-weight: 600;
    padding: 0.6rem 1.8rem 0.6rem 1.8rem;
    font-size: 17px;
}

.btn-2{
    font-weight: 600;
    padding: 0.6rem 1.8rem 0.6rem 1.8rem;
    font-size: 17px;
    color: #e7eee9;
    border: 1px solid #098081;
}

.nav-item{
    a{
        color: #e7eee9;
        text-transform: uppercase;
        font-weight: 600;
        margin: 0 1rem 0 1rem;
        font-size: 17px;
        &:hover{
            border-bottom: 2px solid #bcbdbd;
        }
    }
    
}

.jumbo-text{
    position: absolute;
    width: 40%;
    margin: 0 auto;
    color: white;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
    h1{
        font-size: 80px;
    }
    p{
        font-size: 20px;
        color: #bcbdbd;
    }
}

</style>