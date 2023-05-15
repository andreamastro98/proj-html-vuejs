<script>
    export default{
        name: 'FooterComp'
    }
</script>

<template>
    <div>
        <div class="bg">
            <div class="container-3 row">
                <!-- prima col -->
                <div class="col-3">
                    <div class="mb-3">
                        <span class="logo-1">N E X </span>
                        <span class="logo-2">G E N</span>  
                    </div>

                    <p class="mb-3">A Functional HTML Template for Corporate & Business</p>

                    <div class="mb-3">
                        <span class="me-2"><i class="fa-solid fa-phone"></i></span>
                        <span class="green-text-2">+1(305) 1234-5678</span>
                    </div>
                    <div class="mb-3">
                        <span class="me-2"><i class="fa-solid fa-envelope"></i></span>
                        <span class="green-text-2">hello@example.com</span>
                    </div>
                    <div class="mb-4">
                        <span class="me-2"><i class="fa-solid fa-location-dot"></i></span>
                        <span class="green-text-2">Main Avenue, 987</span>
                    </div>

                    <button type="button" class="btn btn-2">get in touch</button>

                </div>

                <!-- seconda col -->
                <div class="col-3">
                    <div class="card">
                        <h4>About</h4>
                        <ul>
                            <a href=""><li>The Company</li></a>
                            <a href=""><li>Institutional</li></a>
                            <a href=""><li>Social & Events</li></a>
                            <a href=""><li>Innovation</li></a>
                            <a href=""><li>Environment</li></a>
                            <a href=""><li>Technology</li></a>     
                        </ul>
                    </div>
                </div>

                <!-- terza col -->
                <div class="col-3">
                    <div class="card">
                        <h4>Services</h4>
                        <ul>
                            <a href=""><li>Audit & Assurance</li></a>
                            <a href=""><li>Financial Advisory</li></a>
                            <a href=""><li>Analytics M&A</li></a>
                            <a href=""><li>Middle Marketing</li></a>
                            <a href=""><li>Legal Consulting</li></a>
                            <a href=""><li>Regulatory Risk</li></a>      
                        </ul>
                    </div>
                </div>

                <!-- quarta col -->
                <div class="col-3">
                    <div class="card">
                        <h4>Support</h4>
                        <ul>
                            <a href=""><li>Responsability</li></a>
                            <a href=""><li>Terms of Use</li></a>
                            <a href=""><li>About Cookies</li></a>
                            <a href=""><li>Privacy Policy</li></a>
                            <a href=""><li>Accessibility</li></a>
                            <a href=""><li>Information</li></a>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>



<style lang="scss" scoped>

.bg{
    background-image: url(../../public/img/bg-7.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
}

i,span,p,li{
    color: #bcbdbd;
    font-size: 18px;
}

h4{
    color: #bcbdbd;
    margin-bottom: 1rem;
}
.card{
    background-color: rgba(255, 255, 255, 0.05);
    padding: 2rem;
}

ul{
    list-style-type: '> ';
}

a{
   text-decoration: none; 
}

li{
    margin-bottom: 5px;
}

</style>