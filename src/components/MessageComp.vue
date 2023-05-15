<script>
    export default{
        name:'MessageComp'
    }
</script>

<template>
    <div class="container-3">
        <div class="d-flex justify-content-between">
            <div class="width-60">
                <span class="small-green-text">send a message</span>
                <div class="my-4">
                    <span class="span-title">Get in  </span>
                    <span class="green-text span-title">Touch</span>
                </div>
                <p class="mb-4">We will responde to your message as soon as possible.</p>

                <div class="row g-3 mb-3">
                    <div class="col">
                      <input type="text" class="form-control form-control-lg" placeholder="Name" aria-label="name">
                    </div>
                    <div class="col">
                      <input type="text" class="form-control form-control-lg" placeholder="Email" aria-label="email">
                    </div>
                </div>

                <div class="row g-3 mb-3">
                    <div class="col">
                      <input type="text" class="form-control form-control-lg" placeholder="phone" aria-label="phone">
                    </div>
                    <div class="col">
                        <select id="inputState" class="form-select form-select-lg">
                          <option selected>More info</option>
                          <option>...</option>
                        </select>
                    </div>
                </div>

                <div class="form-floating mb-4">
                    <textarea class="form-control" placeholder="Message" id="floatingTextarea2" style="height: 150px"></textarea>
                </div>
                <button type="button" class="btn btn-1">send</button>
            </div>


            <div class="width-35">
                <h2 class="mb-4">Example Inc.</h2>
                <p class="mb-4">Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
                <p class="mb-4">Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
                <div class="mb-3">
                    <span class="me-2"><i class="fa-solid fa-phone round"></i></span>
                    <span class="green-text-2">+1(305) 1234-5678</span>
                </div>
                <div class="mb-3">
                    <span class="me-2"><i class="fa-solid fa-envelope round"></i></span>
                    <span class="green-text-2">hello@example.com</span>
                </div>
                <div class="mb-4">
                    <span class="me-2"><i class="fa-solid fa-location-dot round"></i></span>
                    <span class="green-text-2">Main Avenue, 987</span>
                </div>
                <button type="button" class="btn btn-2" style="color: #098081;">view map</button>
            </div>
        </div>
    </div>
</template>



<style lang="scss" scoped>

.width-60{
    width: 60%;
}
.width-35{
    width: 35%;
}

.width-35>p{
    font-size: 18px;
}

p{
    color: #676669;
    font-size: 17px;
}

.form-control{
    background-color: #ECECEC;
    border: #ECECEC;
    border-radius: 4px;
}

.form-select{
    background-color: #ECECEC;
    border: #ECECEC;
    color: #676669;
    font-size: 17px;
    height: 48px;
    border-radius: 4px;
}

.form-control::placeholder{
    color: #676669;
    font-size: 17px;
}

.green-text-2{
    font-size: 19px;
    color: #098081;

}

</style>