<script setup>
defineProps({
    latest: Array, // Accept the `latest` array as a prop
});
</script>

<template>
    <section>
        <div class="container container-big">
            <div
                class="col-12 d-flex flex-lg-row align-items-center align-items-start align-items-lg-center justify-content-lg-between mb-35px">
                <div class="d-flex flex-column">
                    <p class="sub-title sub-title-lprpl  mb-17px">
                        <slot name="subtitle">Default subtitle</slot>
                    </p>
                    <h3 class="title-1 mb-17px mb-lg-0">
                        <slot name="title">Default title</slot>
                    </h3>
                </div>
                <a href="/" class="btn btn-hovprim btn-md">
                    View All
                </a>
            </div>
            <div class="ev-cont" v-bind="$attrs">
                <!-- Loop through the `latest` array and render an event for each entry -->
                <div v-for="event in latest" :key="event.id" class="event-item">
                    <div class="relative">
                        <img :src="event.src" alt="" class="event-img">
                        <a :href="event.link[0].href" class="stretched-link"></a>
                    </div>
                    <div class="d-flex flex-row flex-wrap-wrap align-items-center mb-10px">
                        <p class="event-date">
                            {{ event.date }}
                        </p>
                        <span class="divider divider-dark"></span>
                        <!-- Loop through categories and render each as a link -->
                        <template v-for="(cat, index) in event.category" :key="index">
                            <a :href="cat.href" class="btn btn-white">
                                {{ cat.title }}
                            </a>
                            <!-- Add a divider between categories (except the last one) -->
                            <span v-if="index < event.category.length - 1" class="divider divider-dark"></span>
                        </template>
                    </div>
                    <h3 class="event-title2">
                        <a :href="event.link[0].href" class="hover-underline">
                            {{ event.link[0].title }}
                        </a>
                    </h3>
                    <a :href="event.link[0].href" class="read-more">
                        Read more
                        <i class="fa fa-arrow-right"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>
</template>
<style scoped lang="scss">
.ev-cont {
    display: grid;
    grid-column-gap: 30px;
    row-gap: 30px;
    grid-template-columns: 1fr;
    align-items: stretch;
    justify-content: center;
    width: 100%;

    @include media-breakpoint-up(md) {
        grid-template-columns: repeat(2, 1fr);
    }

    @include media-breakpoint-up(lg) {
        grid-template-columns: repeat(4, 1fr);

    }
    &-lg-three{
        @include media-breakpoint-up(lg){
            grid-template-columns: repeat(3,1fr);
        }

    }
}

.event-img {
    margin-bottom: 25px;
    width: 100%;
    height: 100%;
    max-height: 270px;
    object-fit: cover;
    position: relative;
    z-index: 1;
    border-radius: inherit;
    filter: grayscale(0%);
}

.event-title2 {
    font-size: 24px;
    line-height: 1.5;
    margin-bottom: 17px;
    font-weight: 500;

}
</style>