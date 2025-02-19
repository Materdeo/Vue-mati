<script>
</script>

<template>
    <div class="event col-12">
        <div class="event-img">
            <a class="link-stretched" href="/">
            </a>
            <img src="/src/assets/images/events-bg-1.jpg" alt="">
        </div>

        <div class="d-flex flex-column mr-auto">
            <h6 class="event-title"><a class="" href="">Bang Pow Boom at Juggaloo island</a></h6>
            <p class="event-date">December 20, 2022</p>
        </div>
        <a class="read-more">
            Manic Depressive
            <i class="fa fa-arrow-right"></i>
        </a>
    </div>
    <div class="event col-12">
        <div class="event-img">
            <a class="link-stretched" href="/">
            </a>
            <img src="/src/assets/images/events-bg-1.jpg" alt="">
        </div>

        <div class="d-flex flex-column mr-auto">
            <h6 class="event-title"><a class="" href="">Bang Pow Boom at Juggaloo island</a></h6>
            <p class="event-date">December 20, 2022</p>
        </div>
        <a class="read-more">
            Manic Depressive
            <i class="fa fa-arrow-right"></i>
        </a>
    </div>
    <div class="event col-12">
        <div class="event-img">
            <a class="link-stretched" href="/">
            </a>
            <img src="/src/assets/images/events-bg-1.jpg" alt="">
        </div>

        <div class="d-flex flex-column mr-auto">
            <h6 class="event-title"><a class="" href="">Bang Pow Boom at Juggaloo island</a></h6>
            <p class="event-date">December 20, 2022</p>
        </div>
        <a class="read-more">
            Manic Depressive
            <i class="fa fa-arrow-right"></i>
        </a>
    </div>

</template>

<style lang="scss" scoped>
.event {
    display: flex;
    flex-direction: column;
    padding-top: 25px;
    margin-bottom: 25px;
    position: relative;

    @include media-breakpoint-up(md) {
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
    }

    &::before {
        height: 1px;
        display: block;
        width: 100%;
        top: 0;
        left: 0;
        right: 0;
        position: absolute;
        content: '';
        background-color: var(--dark);
    }

    &-img {
        max-width: 170px;
        flex-shrink: 0;
        margin-bottom: 20px;
        position: relative;

        @include media-breakpoint-up(lg) {
            margin-right: 30px;
            margin-bottom: 0;
        }
    }

    &-title {
        margin-bottom: 5px;
        font-size: 28px;
        line-height: 36px;
        font-weight: 500;

        a {
            text-decoration: underline;
            text-decoration-color: transparent;
            text-decoration-thickness: 0.08em;
            text-underline-offset: 0.05em;
            transition: all 0.45s;
        }


        @include media-breakpoint-up(lg) {
            margin-bottom: 0;
        }

        &:hover {
            a {
                text-decoration-color: var(--dark);
            }

        }
    }

    &-date {
        font-family: var(--additonal);
        font-weight: 400;
        color: #505558;
        font-size: 12px;
        line-height: 30px;
        text-transform: uppercase;
        margin-bottom: 10px;

        @include media-breakpoint-up(md) {
            margin-bottom: 0;
        }
    }
}
</style>