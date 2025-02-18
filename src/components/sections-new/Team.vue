<script setup></script>
<template>
  <section class="team">
    <div class="container d-flex flex-column">
      <p class="sub-title mb-15px">Our team</p>
      <h3 class="title-1 text-black mb-50px">Meat Great Team</h3>
      <div class="col-12 flex-row team__members">
        <div class="d-flex flex-column">
        <div class="team__item">
          <a href="" class="link-stretched"></a>
          <img class="team__img" src="/src/assets/images/team-1.jpg" alt="" />
          <div class="team__content">
           <a class="morph-btn morph-btn-yellow team__icon" href=""><img src="/src/assets/icons/facebook-circle-white.svg"></img></a>
                    <a class="morph-btn morph-btn-yellow team__icon" href=""><img src="/src/assets/icons/twitter-circle-white.svg"></img></a>
                    <a class="morph-btn morph-btn-yellow team__icon" href=""><img src="/src/assets/icons/instagram-circle-white.svg"></img></a>
          </div>
        </div>
        <div class="d-flex flex-column pt-20px pb-10px">
          <h2 class="team__name">
            Chad Gigacock
          </h2>
          <p class="team__position mt-10px">
            cock in chief
          </p>
        </div>
        </div>
        <div class="d-flex flex-column">
        <div class="team__item">
          <a href="" class="link-stretched"></a>
          <img class="team__img" src="/src/assets/images/team-1.jpg" alt="" />
          <div class="team__content">
           <a class="morph-btn morph-btn-yellow team__icon" href=""><img src="/src/assets/icons/facebook-circle-white.svg"></img></a>
                    <a class="morph-btn morph-btn-yellow team__icon" href=""><img src="/src/assets/icons/twitter-circle-white.svg"></img></a>
                    <a class="morph-btn morph-btn-yellow team__icon" href=""><img src="/src/assets/icons/instagram-circle-white.svg"></img></a>
          </div>
        </div>
        <div class="d-flex flex-column pt-20px pb-10px">
          <h2 class="team__name">
            Chad Gigacock
          </h2>
          <p class="team__position mt-10px">
            cock in chief
          </p>
        </div>
        </div>
        <div class="d-flex flex-column">
        <div class="team__item">
          <a href="" class="link-stretched"></a>
          <img class="team__img" src="/src/assets/images/team-1.jpg" alt="" />
          <div class="team__content">
           <a class="morph-btn morph-btn-yellow team__icon" href=""><img src="/src/assets/icons/facebook-circle-white.svg"></img></a>
                    <a class="morph-btn morph-btn-yellow team__icon" href=""><img src="/src/assets/icons/twitter-circle-white.svg"></img></a>
                    <a class="morph-btn morph-btn-yellow team__icon" href=""><img src="/src/assets/icons/instagram-circle-white.svg"></img></a>
          </div>
        </div>
        <div class="d-flex flex-column pt-20px pb-10px">
          <h2 class="team__name">
            Chad Gigacock
          </h2>
          <p class="team__position mt-10px">
            cock in chief
          </p>
        </div>
        </div>
        <div class="d-flex flex-column">
        <div class="team__item">
          <a href="" class="link-stretched"></a>
          <img class="team__img" src="/src/assets/images/team-1.jpg" alt="" />
          <div class="team__content">
           <a class="morph-btn morph-btn-yellow team__icon" href=""><img src="/src/assets/icons/facebook-circle-white.svg"></img></a>
                    <a class="morph-btn morph-btn-yellow team__icon" href=""><img src="/src/assets/icons/twitter-circle-white.svg"></img></a>
                    <a class="morph-btn morph-btn-yellow team__icon" href=""><img src="/src/assets/icons/instagram-circle-white.svg"></img></a>
          </div>
        </div>
        <div class="d-flex flex-column pt-20px pb-10px">
          <h2 class="team__name">
            Chad Gigacock
          </h2>
          <p class="team__position mt-10px">
            cock in chief
          </p>
        </div>
        </div>
        <div class="d-flex flex-column">
        <div class="team__item">
          <a href="" class="link-stretched"></a>
          <img class="team__img" src="/src/assets/images/team-1.jpg" alt="" />
          <div class="team__content">
           <a class="morph-btn morph-btn-yellow team__icon" href=""><img src="/src/assets/icons/facebook-circle-white.svg"></img></a>
                    <a class="morph-btn morph-btn-yellow team__icon" href=""><img src="/src/assets/icons/twitter-circle-white.svg"></img></a>
                    <a class="morph-btn morph-btn-yellow team__icon" href=""><img src="/src/assets/icons/instagram-circle-white.svg"></img></a>
          </div>
        </div>
        <div class="d-flex flex-column pt-20px pb-10px">
          <h2 class="team__name">
            Chad Gigacock
          </h2>
          <p class="team__position mt-10px">
            cock in chief
          </p>
        </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
  .team {
    padding: 80px 0;
    @include media-breakpoint-up(lg) {
      padding: 121px 0;
    }
    &__members {
      display: grid;
      grid-template-columns: repeat(5, auto);
      grid-column-gap: 30px;
    }
    &__item {
      position: relative;
      display: flex;
      &::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        border-radius: inherit;
        transition: 0.3s;
      }
      &::after {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        border-radius: inherit;
        transition: 0.3s;
        background: rgba(0, 0, 0, 0.5);
        opacity: 0;
      }
      &:hover {
        &::after {
          opacity: 1;
        }
        .team__content{
          opacity: 1;
        }
      }
    }
    &__icon{
        width: 50px;
        height: 50px;
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        img{
            width: 28px;
            height: 28px;
        }
    }
    &__img {
    }
    &__link {
    }
    &__content {
      position: absolute;
      z-index: 1;
      display: flex;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      transition: 0.3s;
      opacity: 0;
    }
    &__name{
      font-size: 24px;
  line-height: 1.3;
  font-weight: 500;

    }
    &__position{
font-size: 12px;
  font-weight: 400;
  line-height: 1;
  text-transform: uppercase;
    }
  }
</style>
