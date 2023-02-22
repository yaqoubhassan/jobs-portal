<template>
    <section class="section-box pt-5">
        <div class="banner-hero hero-2">
            <div class="banner-inner">
                <div class="block-banner">
                    <h1 class="text-42 color-white" style="visibility: visible; animation-name: fadeInUp;">The #1 <span
                            class="color-green">Job Board for</span><br class="d-none d-lg-block"> Hiring or Find your next
                        job</h1>
                    <div class="banner-description color-white mt-4" data-wow-delay=".1s"
                        style="visibility: visible; animation-delay: 0.1s; animation-name: fadeInUp;">Each month, more than
                        3
                        million job seekers turn to website in their search for work, making over 140,000 applications every
                        single
                        day
                    </div>
                    <app-hero-search-area></app-hero-search-area>
                    <div class="mt-3">
                        <p>
                            <strong class="popular-searches strong-text">Popular Searches:</strong>
                            <a class="popular-searches" href="#">Designer</a>
                            <a class="popular-searches" href="#">Web</a>
                            <a class="popular-searches" href="#">IOS</a>
                            <a class="popular-searches" href="#">Developer</a>
                            <a class="popular-searches" href="#">PHP</a>
                            <a class="popular-searches" href="#">Senior</a>
                            <a class="popular-searches" href="#">Engineer</a>
                        </p>
                    </div>
                    <div class="row my-5 stats">
                        <div class="col-xl-3 col-lg-3 col-md-3 col-sm-6">
                            <h4>245K+</h4>
                            <p>Daily Jobs Posted</p>
                        </div>
                        <div class="col-xl-3 col-lg-3 col-md-3 col-sm-6">
                            <h4>300K+</h4>
                            <p>Recruiters</p>
                        </div>
                        <div class="col-xl-3 col-lg-3 col-md-3 col-sm-6">
                            <h4>578K+</h4>
                            <p>Freelancers</p>
                        </div>
                        <div class="col-xl-3 col-lg-3 col-md-3 col-sm-6">
                            <h4>120K+</h4>
                            <p>Blog Tips</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import HeroSearchArea from './HeroSearchArea.vue'

export default {
    components: {
        appHeroSearchArea: HeroSearchArea
    }
}
</script>

<style scoped>
.banner-hero.hero-2 {
    position: relative;
    width: 100%;
    padding: 100px 0px 80px 0px;
    max-width: 100%;
    background: url('../assets/banner.png') no-repeat top center;
    background-size: cover;
}

.banner-hero.hero-2::before {
    content: "";
    position: absolute;
    top: 0px;
    left: 0px;
    width: 100%;
    height: 100%;
    background-color: #05264E;
    opacity: 0.8;
    z-index: 1;
}

.banner-hero.hero-2 .banner-inner {
    z-index: 2;
    position: relative;
    max-width: 725px;
    margin: auto;
    width: 100%;
}

.banner-hero .banner-inner {
    padding-left: 15px;
    padding-right: 15px;
}

.banner-hero.hero-2 .banner-inner .block-banner {
    padding: 0px;
    text-align: center;
}

.text-42 {
    font-size: 42px;
    line-height: 53px;
    font-weight: 700;
}

.color-white {
    color: #ffffff !important;
}

.color-green {
    color: #85FF83;
}

.banner-description {
    font-weight: 400;
    font-size: 18px;
    line-height: 26px;
    font-family: "Plus Jakarta Sans", sans-serif;
    font-style: normal;
}

.popular-searches {
    color: #ffffff;
    font-size: 14px;
    margin: 0px 5px;
}

@media (min-width: 576px) {
    .offset-sm-4 {
        margin-left: 0px;
    }
}

@media (max-width:768px) {
    .strong-text {
        display: block
    }
}

.stats h4 {
    color: #FFFFFF;
    font-weight: 700;
    /* letter-spacing: .2rem; */
}

.stats p {
    color: #A0ABB8;
}

#jobs-section p {
    font-weight: 500;
    font-size: 18px;
    line-height: 26px;
    color: #66789C;
}

.center-align {
    float: center !important;
    margin-left: 40px;
}
</style>