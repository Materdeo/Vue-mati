<script setup>
import UpcomingEvents from '@/components/sections/UpcomingEvents.vue';
import MainFooter from '@/components/sections-new/MainFooter.vue';
import Team from '@/components/sections-new/Team.vue';
import Services from '@/components/sections-new/Services.vue'
import CategoriesImg from '@/components/sections-new/Categories-img.vue';
import Events from '@/components/sections-new/Events.vue'



const team = [
  {
    id: 1,
    teamImg: '/src/assets/images/team-1.jpg',
    teamLink: '/chad',
    teamLinkFb: '/fb',
    teamLinkTw: '/tw',
    teamLinkIns: '/ins',
    teamName: 'Chad Gigacock',
    teamProps: 'HNIC',
  },
  {
    id: 2,
    teamImg: '/src/assets/images/team-1.jpg',
    teamLink: '/chad',
    teamLinkFb: '/fb',
    teamLinkTw: '/tw',
    teamLinkIns: '/ins',
    teamName: 'Chad Gigacock',
    teamProps: 'HNIC',
  },
  {
    id: 3,
    teamImg: '/src/assets/images/team-1.jpg',
    teamLink: '/chad',
    teamLinkFb: '/fb',
    teamLinkTw: '/tw',
    teamLinkIns: '/ins',
    teamName: 'Chad Gigacock',
    teamProps: 'HNIC',
  },
  {
    id: 4,
    teamImg: '/src/assets/images/team-1.jpg',
    teamLink: '/chad',
    teamLinkFb: '/fb',
    teamLinkTw: '/tw',
    teamLinkIns: '/ins',
    teamName: 'Chad Gigacock',
    teamProps: 'HNIC',
  },
  {
    id: 5,
    teamImg: '/src/assets/images/team-1.jpg',
    teamLink: '/chad',
    teamLinkFb: '/fb',
    teamLinkTw: '/tw',
    teamLinkIns: '/ins',
    teamName: 'Chad Gigacock',
    teamProps: 'HNIC',
  },
];
</script>

<template>
  <h1>ZMIEŃ WSZYSTKIE KLAS- na KLAS__ you mongrel</h1>
  <CategoriesImg class="pt-70px pt-lg-120px pb-60px pb-lg-90px" />
  <section>
    <div class="container flex-column align-items-center">
      <p class="sub-title sub-title-lprpl mb-20px">FUTURE EVENTS</p>
      <h3 class="title-1 mb-20px">Festivals This December </h3>
      <Events />
    </div>
  </section>
  <Services />
  <Team :team="team">
    <template #subtitle>Meet Our Team</template>
    <template #title>Our Professionals</template>
  </Team>
</template>