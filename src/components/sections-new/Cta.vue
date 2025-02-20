<script setup>

</script>

<template>
    <div class="cta-scroller">
        <div class="d-flex flex-row align-items-center">
            <span>Future Events</span>
            <i class="fa fa-arrow-down"></i>
        </div>
        <div class="d-flex flex-row align-items-center">
            <span>Future Events</span>
            <i class="fa fa-arrow-down"></i>
        </div>
        <div class="d-flex flex-row align-items-center">
            <span>Future Events</span>
            <i class="fa fa-arrow-down"></i>
        </div>
        <div class="d-flex flex-row align-items-center">
            <span>Future Events</span>
            <i class="fa fa-arrow-down"></i>
        </div>
        <div class="d-flex flex-row align-items-center">
            <span>Future Events</span>
            <i class="fa fa-arrow-down"></i>
        </div>
        <div class="d-flex flex-row align-items-center">
            <span>Future Events</span>
            <i class="fa fa-arrow-down"></i>
        </div>
        <div class="d-flex flex-row align-items-center">
            <span>Future Events</span>
            <i class="fa fa-arrow-down"></i>
        </div>
        <div class="d-flex flex-row align-items-center">
            <span>Future Events</span>
            <i class="fa fa-arrow-down"></i>
        </div>
        <div class="d-flex flex-row align-items-center">
            <span>Future Events</span>
            <i class="fa fa-arrow-down"></i>
        </div>

        <div class="d-flex flex-row align-items-center">
            <span>Future Events</span>
            <i class="fa fa-arrow-down"></i>
        </div>

    </div>
    <section class="pt-40px pt-lg-130px  pb-50px pb-lg-105px cta">
        <div class="container container-big">
            <div class="cta-left">
                <p class="sub-title mb-17px">
                    Lorem ipsum
                </p>
                <h3 class="cta-title mb-20px">
                    The Essential Guide to Upcoming Festivals
                </h3>
                <p class="mb-35px text-gray">
                    Facilisi etiam dignissim diam quis sociis natoque penatibus. Aliquam ut porttitor leo a diam
                    sollicitudin velit sed ullamcorper morbi porta non pulvinar neque.
                </p>
                <a class="btn btn-md morph-outline" href="">
                    Learn more
                </a>
            </div>
            <div class="cta-right">

            </div>
        </div>
        <div class="cta-cloud">
            <img src="/src/assets/images/cta-cloud.png" alt="">
        </div>
        <div class="cta-calendar">
            zmień nazwe
            <img src="/src/assets/images/cat-calendar.png" alt="">
        </div>
    </section>
</template>

<style lang="scss" scoped>
.cta {
    column-gap: 30px;
    background-color: var(--primary);
    background-image: url("src/assets/images/cta-bg.jpg");
    background-position: center right;
    background-repeat: no-repeat;
    overflow: hidden;

    &-left {
        display: flex;
        flex-direction: column;

        @include media-breakpoint-up(lg) {}

        width: 44%;
    }

    &-right {
        display: flex;
        flex-direction: column;

        @include media-breakpoint-up(lg) {}

        width: 56%;
    }

    &-scroller {
        background-color: var(--primary);
        width: 100%;
        padding: 18px 0;
        display: flex;
        flex-direction: row;
        border: 1px solid var(--text);
        border-left: 0;
        border-right: 0;
        white-space: nowrap;

        span {
            text-transform: uppercase;
            font-family: var(--addtional);
            font-weight: 400;
            letter-spacing: 0.16px;
            line-height: 30px
        }

        i {
            margin-right: 38px;
            margin-left: 32px;
            color: var(--text);
            display: inline-block;
            position: relative;
            vertical-align: middle;
            font-size: 16px;
            font-weight: 400;
        }

    }

    &-title {
        font-size: 26px;
        line-height: 1.24em;
        font-weight: 500;

        @include media-breakpoint-up(md) {
            font-size: 58px;

        }
    }

    &-cloud {
        position: absolute;
        transform: translateY(-32px);
        transition: transform linear;
        will-change: transform;
        opacity: 1;
        visibility: visible;
        width: 100%;
        z-index: 1;

        @include media-breakpoint-up(lg) {
            top: 45%;
            left: 25%;
        }

    }

    &-calendar {
        position: absolute;
        z-index: 0;
        width: 100%;
        pointer-events: none;
        transform: translateX(-20px);
        transition: transform linear;
        will-change: transform;
        opacity: 1;
        visibility: visible;

    }

}
</style>