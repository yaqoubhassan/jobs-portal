<template>
  <app-header></app-header>
  <main class="main">
    <app-hero></app-hero>
    <section class="mt-5" id="jobs-section">
      <div class="container">
        <div class="text-center">
          <h2 style="color: #05264E; font-weight: 700; font-size: 36px;">Jobs of the Day</h2>
          <p>Search and connect with the right candidates faster.</p>

          <div class="list-tabs mt-4 center-align">
            <ul class="nav nav-tabs ms-auto me-auto">
              <li><a class="" id="nav-tab-job-1" href="#tab-job-1" data-bs-toggle="tab" role="tab"
                  aria-controls="tab-job-1" aria-selected="false"><img src="./assets/management.svg" alt="jobBox">
                  Management</a>
              </li>
              <li><a id="nav-tab-job-2" href="#tab-job-2" data-bs-toggle="tab" role="tab" aria-controls="tab-job-2"
                  aria-selected="false" class=""><img src="./assets/marketing.svg" alt="jobBox"> Marketing
                  &amp; Sale</a></li>
              <li><a id="nav-tab-job-3" href="#tab-job-3" data-bs-toggle="tab" role="tab" aria-controls="tab-job-3"
                  aria-selected="false" class=""><img src="./assets/finance.svg" alt="jobBox"> Finance</a>
              </li>
              <li><a id="nav-tab-job-4" href="#tab-job-4" data-bs-toggle="tab" role="tab" aria-controls="tab-job-4"
                  aria-selected="false" class=""><img src="./assets/human.svg" alt="jobBox"> Human
                  Resource</a></li>
              <li><a id="nav-tab-job-5" href="#tab-job-5" data-bs-toggle="tab" role="tab" aria-controls="tab-job-5"
                  aria-selected="false" class=""><img src="./assets/retail.svg" alt="jobBox"> Retail &amp;
                  Products</a></li>
              <li><a id="nav-tab-job-6" href="#tab-job-6" data-bs-toggle="tab" role="tab" aria-controls="tab-job-6"
                  aria-selected="true" class="active"><img src="./assets/content.svg" alt="jobBox">
                  Content Writer</a></li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <div style="height: 700px"></div>


  </main>
</template>

<script>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'

export default {
  components: {
    appHeader: Header,
    appHero: Hero
  }
}

</script>

<style>
body {
  background-color: #FFFFFF;
  font-family: "Plus Jakarta Sans", sans-serif;
}

.center-align {
  margin-left: 40px;
}

.nav-tabs li {
  margin: auto;
}

.nav-tabs li a {
  display: block;
  margin: 0px 5px;
  box-shadow: 0px 2px 4px -5px rgb(10 42 105);
  align-items: center;
  padding: 13px 17px;
  width: auto;
  background: #ffffff;
  border: 1px solid #E0E6F7;
  border-radius: 8px;
  font-family: "Plus Jakarta Sans", sans-serif;
  font-size: 12px;
  font-weight: 700;
  line-height: 18px;
  text-align: left;
  margin-bottom: 10px;
  text-decoration: none;
  color: #05264E;
}

.nav-tabs li a:hover {
  border: 1px solid #3C65F5;
}

</style>
