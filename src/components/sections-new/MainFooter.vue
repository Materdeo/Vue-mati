<script setup>

</script>

<template>
    <section class="footer">
        <div class="container">
            <div class="col-12 col-lg-3 d-flex flex-column">

            </div>
            <div class="col-12 col-lg-6 d-flex flex-column">
                <img class="footer__logo mb-25px" src="/src/assets/images/logo-white.png" alt="">
                <p class="text-center mb-25px">We help organisations transform their impact by providing a comprehensive new great experience </p>
                <div class="d-flex flex-row justify-content-center"><a class="text-white hover-primary" href="/">Privacy Policy</a><span class="text-white divider ">|</span><a class="text-white hover-primary" href="/">Terms of use</a></div>
                <div class="d-flex flex-row justify-content-between">
                    <a class="morph footer__icon" href=""><i class="fa fa-ethereum"></i></a>
                </div>

            </div>
            <div class="col-12 col-lg-3 d-flex flex-column">

            </div>
        </div>
    </section>

</template>

<style  lang="scss">
.footer{
    background-color:var(--footer);

    padding: 60px 0px 60px 0px;
    @include media-breakpoint-up(md){
        padding: 80px 0px 70px 0px;
    }
    @include media-breakpoint-up(xl){
        padding: 80px 15px 70px 15px;
    }
    &__logo{
        height: 60px;
        object-fit: cover;
        width: fit-content;
    }
    &__icon{
        padding: 25px 14px 25px 14px;
        background-color: #FFF0;
        .fa{
            font-size: 30px;
            color: white;
        }
        position: relative;
        &::after{

        }
    }

    
}
</style>