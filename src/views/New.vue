<script setup>
import UpcomingEvents from '@/components/sections/UpcomingEvents.vue';
import MainFooter from '@/components/sections-new/MainFooter.vue';
import Team from '@/components/sections-new/Team.vue';
import Services from '@/components/sections-new/Services.vue'
import CategoriesImg from '@/components/sections-new/Categories-img.vue';
import Events from '@/components/sections-new/Events.vue'
import LatestEvents from '@/components/sections-new/LatestEvents.vue';
import Cta from '@/components/sections-new/Cta.vue';



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
const latest = [
  {
    id: 1,
    src: '/src/assets/images/bangpow.jpg',
    link: [
      {
        href: '/icp',
        title: 'Bang Pow Boom at Jugaloo Island'
      }
    ],
    category: [
      {
        href: '/bpb',
        title: 'BangPow'
      },
    ],
    date: 'January 22, 2025'
  },
  {
    id: 2,
    src: '/src/assets/images/greatmilenko.jpg',
    link: [{ href: '/icp', title: 'Great MILENKO GREAT MILENKO' }],
    date: 'January 22, 2025',
    category: [{
      href: '/bpb',
      title: 'greatmilenko'
    }],
  },
  {
    id: 3,
    src: '/src/assets/images/hellspit.jpg',
    link: [{ href: '/icp', title: 'GIVE ME HEAD BIIITCH' }],
    date: 'January 22, 2025',
    category: [{
      href: '/bpb',
      title: 'Hellspit'
    }],
  },
  {
    id: 4,
    src: '/src/assets/images/Jeckelbros.jpg',
    link: [{ href: '/icp', title: 'Jeckelbross' }],
    date: 'January 22, 2025',
    category: [{
      href: '/bpb',
      title: 'Jeckelbros'
    }],
  },

]
const events = [
  {
    id: 1,
    src: '/src/assets/images/events-bg-1.jpg',
    mainLink: [
      {
        href: '/icp',
        title: 'Bang pow boom at jugaloo island',
        location: 'Jugaloo Island'
      }
    ],
    date: '22.02.2025',
  },
  {
    id: 2,
    src: '/src/assets/images/events-bg-1.jpg',
    mainLink: [
      {
        href: '/icp',
        title: 'Proponent for sentience',
        location: 'Alleagon'
      }
    ],
    date: '22.02.2025',
  },
];
</script>

<template>
  <Hero />
  <h1 class="pb-100px">ZMIEŃ WSZYSTKIE KLAS- na KLAS__ you mongrel, WIĘKSZE SPANY W ANIM TEXT</h1>
  <h3>todo jak wróce</h3>
  <Cta />
  <LatestEvents :latest="latest">
    <template #subtitle>Insane Clown Posse</template>
    <template #title>Latest updates from the best band</template>
  </LatestEvents>

  <CategoriesImg class="pt-70px pt-lg-120px pb-60px pb-lg-90px" />
  <section class="pb-75px">
    <div class="container flex-column align-items-center">
      <p class="sub-title sub-title-lprpl mb-20px">FUTURE EVENTS</p>
      <h3 class="title-1 mb-20px">Festivals This December </h3>
      <Events v-for="event in events" v-bind="event" :key="event.id" />
    </div>
  </section>
  <Services />
  <Team :team="team">
    <template #subtitle>Meet Our Team</template>
    <template #title>Our Professionals</template>
  </Team>
</template>