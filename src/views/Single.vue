<script setup>
import HeroSmall from '@/components/sections-new/Hero-small.vue';
</script>

<template>
  <HeroSmall source="/src/assets/images/blog-bg.jpg" title="Single" />
  <section class="single">
    <div class="container container-small">
        <div class="single__content">
            <div class="single__intro">
                <img src="" alt="">
            </div>
            <h1 class="single__title">

            </h1>
            <div class="single__details">
                <div>
                    <h6>Event date:</h6>
                    <p>
                        Start at 12:00 AM
                        December 27, 2022 - December 29, 2022 </p>
                </div>
                <div>
                    <h6>Location:</h6>
                    <p>GERMANY</p>
                </div>
                <div>
                    <h6>E-mail:</h6>
                    <p>
                        <a class="hover-none" href="">city@vox.com.ua</a>
                        <a class="hover-none" href="">thegov@gmail.com</a>
                    </p>
                </div>

            </div>
            <h4>

            </h4>

        </div>
        
    </div>
  </section>
</template>


<style scoped lang="scss">
.single{
    &__intro{

    }
    &__title{

    }
    &__details{
        h6{

        }
        p{

        }

    }
    
}


</style>