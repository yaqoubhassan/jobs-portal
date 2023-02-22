<template>
  <app-header></app-header>
  <main class="main">
    <app-hero></app-hero>
    <app-jobs-section></app-jobs-section>

    <div style="height: 700px"></div>


  </main>
</template>

<script>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import JobsSection from './components/JobsSection.vue';

export default {
  components: {
    appHeader: Header,
    appHero: Hero,
    appJobsSection: JobsSection
  }
}

</script>

<style>
body {
  background-color: #FFFFFF;
  font-family: Candara, sans-serif;
}
</style>
