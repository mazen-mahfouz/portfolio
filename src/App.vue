<template>
  <div id="app" :class="{'light bg-[linear-gradient(360deg,_rgb(244,_247,_252),_rgb(255,_255,_255))]': $store.state.them == 'light', 'dark bg-[linear-gradient(360deg,_rgb(7,_11,_22),_rgb(15,_23,_42))]': $store.state.them == 'dark'}">
      <NavPage />
      <HeaderPage />
      <SkillsPage />
      <ProjectPage />
      <ContactusPage />
      <FooterPage />
  </div>
</template>

<script>

import NavPage from './components/NavPage.vue'
import HeaderPage from './components/HeaderPage.vue'
import SkillsPage from './components/SkillsPage.vue'
import ProjectPage from './components/ProjectPage.vue'
import FooterPage from './components/FooterPage.vue'
import ContactusPage from './components/ContactusPage.vue'

export default {
  name: 'App',
  components: {
    NavPage,
    ProjectPage,
    FooterPage,
    ContactusPage,
    SkillsPage,
    HeaderPage
  },


}
</script>

<style lang="scss">
.ar{
      flex-direction: row-reverse;
      text-align: right;
      
      h1, ul, p{
        text-align: right;
      }
  }
  .en{
      flex-direction: row;
      text-align: left;
  }
</style>
