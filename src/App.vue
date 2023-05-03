<script setup>
import Carousel1 from "./components/Carousel1.vue"
import Carousel2 from "./components/Carousel2.vue"
import Carousel3 from "./components/Carousel3.vue"
</script>

<script>
export default {
    name: "App"
}
</script>

<template>
    <div class="wrapper">
        <div class="top-nav-wrapper">
            <nav class="top-nav">
                <div class="top-left-nav">
                    <div class="top-left-nav-btn selected-btn">Students</div>
                    <div class="top-left-nav-btn">Employers</div>
                    <div class="top-left-nav-btn">Career Centers</div>
                </div>

                <div>
                    <div class="top-right-nav-btn">Log in</div>
                </div>
            </nav>
        </div>

        <div class="second-nav-wrapper">
            <nav class="second-nav">
                <div style="padding: 5px">
                    <img src="./assets/images/logos/handshake.svg" />
                </div>

                <div class="second-nav-btns">
                    <div class="second-nav-btn selected-btn-2">Overview</div>
                    <div class="second-nav-btn">How it works</div>
                    <div class="second-nav-btn">Who's hiring</div>
                    <div class="second-nav-btn">Career tips</div>

                    <button
                        class="sign-up-btn"
                        style="font-size: 12pt; margin-left: 10px"
                    >
                        Sign up
                    </button>
                </div>
            </nav>
        </div>

        <div class="whos-hiring-section-wrapper">
            <section class="whos-hiring-section">
                <strong>We're hiring for our team! </strong>Explore open roles
                on Handshake.
            </section>
        </div>

        <div class="sign-up-responsive-wrapper">
            <section class="sign-up-wrapper">
                <div class="sign-up-info-wrapper">
                    <div class="number-one-title">
                        The #1 way college students get hired
                    </div>

                    <div style="font-size: 18pt; margin-top: 20px">
                        Meet people who help you land the job
                    </div>

                    <div style="margin-top: 20px">
                        <input
                            type="text"
                            placeholder="Type .edu email here"
                            class="edu-input"
                        />
                        <button class="sign-up-btn" >
                            Sign up
                        </button>
                    </div>
                </div>

                <img src="./assets/images/hero.png" class="hero-img" />
            </section>
            <img
                src="./assets/images/hero--desktop.png"
                alt="hero-desktop"
                class="desktop-hero-img"
            />
        </div>

        <section class="launch-wrapper">
            <div class="launch-heading">
                Launch your career <br />on Handshake
            </div>

            <div class="launch-card-wrapper">
                <div class="launch-card">
                    <img src="./assets/images/front-page-right-jobs-icon.png" />
                    <div class="launch-text">The right jobs for you</div>
                </div>

                <div class="launch-card">
                    <img src="./assets/images/front-page-one-on-one-icon.png" />
                    <div class="launch-text">
                        One-on-one convos with employers
                    </div>
                </div>

                <div class="launch-card">
                    <img src="./assets/images/front-page-work-exp-icon.png" />

                    <div class="launch-text">No work experience required</div>
                </div>
            </div>

            <div class="how-it-works-btn-wrapper">
                <button class="how-it-works-btn">How it works</button>
            </div>
        </section>

        <section class="hiring-section">
            <div class="hiring-content">
                <div class="hiring-heading">Meet top employers hiring now</div>
                <button class="whos-hiring-btn">Who's hiring</button>
            </div>

            <div class="hiring-img-wrapper">
                <img
                    style="position: relative; top: 0; left: 0"
                    src="./assets/images/purple-squiggle.png"
                    height="400px"
                />
                <img
                    style="position: absolute; top: 40px; left: 80px"
                    src="./assets/images/front-page-meet-top-employers.png"
                    height="300px"
                />
            </div>
        </section>

        <section class="hiring-section-mobile">
            <div class="hiring-heading">Meet top employers hiring now</div>

            <div class="hiring-img-wrapper">
                <img
                    style="position: relative; top: 0; left: 0"
                    src="./assets/images/purple-squiggle.png"
                    height="400px"
                />
                <img
                    style="position: absolute; top: 40px; left: 80px"
                    src="./assets/images/front-page-meet-top-employers.png"
                    height="300px"
                />
            </div>

            <button class="whos-hiring-btn">Who's hiring</button>
        </section>

        <section class="carousel-wrapper">
            <Carousel1 />
            <Carousel2 />
            <Carousel3 />
            <Carousel1 class="extra-carousel" />
        </section>
    </div>
</template>

<style scoped>
@font-face {
    font-family: "sansplomb";
    src: url(../src/assets/plomb/SansPlomb_TRIAL-95.otf);
}

.top-left-nav {
    display: flex;
    flex-direction: row;
}
.top-nav {
    background-color: black;
    color: white;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}

.second-nav {
    padding: 15px;
    display: flex;
    justify-content: center;
}

.top-left-nav-btn {
    padding-left: 20px;
    padding-right: 20px;
    padding-top: 15px;
    padding-bottom: 15px;
    cursor: pointer;
    font-size: 10pt;
}

.top-left-nav-btn:hover {
    border-bottom: 5px solid white;
}

.selected-btn {
    border-bottom: 5px solid white;
}

.number-one-title {
    font-family: "sansplomb";
}

.selected-btn-2 {
    border-bottom: 5px solid rgb(144, 78, 238);
}

.top-right-nav-btn {
    padding-left: 20px;
    padding-right: 20px;
    padding-top: 15px;
    padding-bottom: 15px;
    font-size: 10pt;
}

.top-right-nav-btn:hover {
    cursor: pointer;
    border-bottom: 5px solid white;
}

.sign-up-btn {
    background-color: black;
    color: white;
    border-radius: 5px;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
    font-size: 14pt;
}

.whos-hiring-section {
    text-align: center;
    padding: 20px;
    font-size: 12pt;
    background-color: rgb(243, 245, 254);
}

.edu-input {
    padding: 10px;
    border-radius: 5px;
    border: none;
    margin-right: 15px;
}

.second-nav-btn {
    padding-top: 10px;
    padding-bottom: 10px;
    margin-left: 10px;
    margin-right: 10px;
    cursor: pointer;
    font-size: 12pt;
}

.second-nav-btn:hover {
    border-bottom: 5px solid rgb(144, 78, 238);
}

.second-nav-btns {
    display: none;
}

.hiring-heading {
    font-size: 24pt;
    padding: 20px;
    width: 300px;
}

.sign-up-wrapper {
    display: flex;
    flex-direction: column;
    background-color: rgb(206, 249, 91);
}

.sign-up-info-wrapper {
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 20px;
}

.desktop-hero-img {
    height: 580px;
    float: right;
}

.number-one-title {
    font-size: 42pt;
    font-weight: bold;
}

.launch-card {
    width: 200px;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.launch-text {
    text-align: center;
    margin-top: 10px;
    margin-bottom: 10px;
    font-size: 18pt;
}

.launch-heading {
    display: flex;
    justify-content: center;
    font-size: 30pt;
    text-align: center;
    padding: 50px;
}

.how-it-works-btn {
    background-color: black;
    color: white;
    border-radius: 5px;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
}

.how-it-works-btn-wrapper {
    display: flex;
    justify-content: center;
    padding: 25px;
}

.whos-hiring-btn {
    background-color: black;
    color: white;
    border-radius: 5px;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
    width: fit-content;
    margin: 20px;
}

.carousel-wrapper {
    display: flex;
    justify-content: center;
}

.launch-card-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 0 auto;
}

.hiring-section-mobile {
    display: flex;
    flex-direction: column;
    text-align: center;
    align-items: center;
    padding: 10px;
}

.hiring-section {
    display: none;
    flex-direction: row;
    justify-content: center;
    padding: 50px;
}

.hiring-content {
    display: flex;
    flex-direction: column;
    justify-content: center;
}

.hiring-img-wrapper {
    position: relative;
    top: 0;
    left: 0;
    width: fit-content;
}

.desktop-hero-img {
    display: none;
}

.extra-carousel {
    display: none;
}

/* applies on large screens. */
@media screen and (min-width: 1240px) {
    .launch-card-wrapper {
        flex-direction: row;
        width: 800px;
        justify-content: space-between;
    }

    .sign-up-wrapper {
        position: absolute;
        width: 1240px;
        top: 50%;
        z-index: 1;
        left: 50%;
        transform: translate(-50%, -50%);
        height: 100%;

    }

    .sign-up-info-wrapper {
        height: 100%;
        width: 500px;
    }

    .number-one-title {
        font-size: 70pt;
    }
    .hero-img {
        display: none;
    }

    .desktop-hero-img {
        display: block;
        z-index: 2;
    }

    .extra-carousel {
        display: block;
    }

    .second-nav {
        justify-content: space-between;
        width: 1240px;
    }

    .whos-hiring-section {
        width: 1240px;
    }

    .second-nav-btns {
        display: flex;
    }

    .hiring-section {
        display: flex;
    }

    .hiring-section-mobile {
        display: none;
    }

    .top-nav {
        width: 1240px;
    }

    .top-nav-wrapper {
        background-color: black;
        display: flex;
        justify-content: center;
    }

    .second-nav-wrapper {
        display: flex;
        justify-content: center;
    }

    .whos-hiring-section-wrapper {
        display: flex;
        justify-content: center;
        background-color: rgb(243, 245, 254);
    }

    .sign-up-responsive-wrapper {
        display: flex;
        justify-content: flex-end;
        position: relative;
    background-color: rgb(206, 249, 91);

    }
}
</style>
