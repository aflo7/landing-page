<script setup>
import Carousel1 from "./components/Carousel1.vue"
import Carousel2 from "./components/Carousel2.vue"
import Carousel3 from "./components/Carousel3.vue"
import App2 from "./components/App2.vue"
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
                <div style="padding-top: 5px; padding-left: 10px;">
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
                        <button class="sign-up-btn">Sign up</button>
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

        <div class="launch-heading">Launch your career <br />on Handshake</div>

        <div class="launch-card-wrapper">
            <div class="launch-card">
                <img src="./assets/images/front-page-right-jobs-icon.png" />
                <div class="launch-text">The right jobs for you</div>
            </div>

            <div class="launch-card">
                <img src="./assets/images/front-page-one-on-one-icon.png" />
                <div class="launch-text">One-on-one convos with employers</div>
            </div>

            <div class="launch-card">
                <img src="./assets/images/front-page-work-exp-icon.png" />

                <div class="launch-text">No work experience required</div>
            </div>
        </div>

        <div class="how-it-works-btn-wrapper">
            <button class="how-it-works-btn">How it works</button>
        </div>

        <div class="hiring-section-wrapper">
            <section class="hiring-section">
                <div class="hiring-content">
                    <div class="hiring-heading">
                        Meet top employers hiring now
                    </div>
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
        </div>

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

        <div class="recruiter-wrapper">
            <div class="recruiter-content">
                <img
                    src="./assets/images/hired-on-handshake.png"
                    class="hired-on-handshake-img"
                />
                <h1 class="recruiter-heading">Recruiters find you</h1>

                <div class="student-info-wrapper">
                    <div class="student-info">
                        <p>
                            "A recruiter at eBay reached out to me directly and
                            encouraged me to apply. Applying was easy and I knew
                            exactly what they were looking for."
                        </p>

                        <p>Amisha, UC Berkeley</p>
                    </div>

                    <div class="student-img-container">
                        <img src="./assets/images/amisha.jpg" />
                    </div>
                </div>

                <div class="student-info-wrapper student-info-wrapper-reverse">
                    <div class="student-info">
                        <p>
                            "Within one week of creating my profile—one week!—I
                            was invited to interview for Dell Technologies. And
                            I got a job!"
                        </p>

                        <p>James, Boston University</p>
                    </div>

                    <div class="student-img-container">
                        <img src="./assets/images/james.jpg" />
                    </div>
                </div>

                <div class="student-info-wrapper">
                    <div class="student-info">
                        <p>
                            "One day I got an email in my inbox saying you have
                            a message from Microsoft. It was an invitation to
                            interview!"
                        </p>

                        <p>Ami, UC Irvine</p>
                    </div>

                    <div class="student-img-container">
                        <img src="./assets/images/ami.jpg" />
                    </div>
                </div>
            </div>
        </div>

        <div class="first-to-know-wrapper">
            <div class="first-to-know-content">
                <div class="first-to-know-info">
                    <h1>Be the first to know</h1>
                    <p>
                        The freshest full-time jobs, internships, and
                        connections
                    </p>
                </div>
            </div>
        </div>

        <App2 />
    </div>
</template>

<style scoped>

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
    padding-top: 20px;
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



.selected-btn-2 {
    border-bottom: 5px solid rgb(144, 78, 238);
}

.top-right-nav-btn {
    padding-left: 20px;
    padding-right: 20px;
    padding-top: 20px;
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
    font-family: "sansplomb";

}

.launch-card {
    padding-bottom: 20px;
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
    padding-top: 20px;
    padding-bottom: 20px;
}

.launch-card-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
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
    padding: 60px;
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

.recruiter-content {
    background-color: rgb(10, 32, 34);
    color: white;
    margin-top: 80px;
    position: relative;
}

.recruiter-heading {
    padding-top: 120px;
    padding-bottom: 20px;
    text-align: center;
    font-size: 22pt;
}

.hired-on-handshake-img {
    width: 150px;
    position: absolute;
    top: 0%;
    left: 50%;
    transform: translate(-50%, -50%);
}

.student-info-wrapper {
    padding: 30px;
    padding-left: 50px;
    padding-right: 50px;
}
.student-img-container {
    overflow: hidden;
    transform: skew(-3deg);
    display: inline-block;
    background-color: white;
}
.student-img-container img {
    transform: skew(3deg);
    display: block;
    width: 200px;
}

.first-to-know-content {
    height: 800px;
    display: flex;
    justify-content: center;
}

.first-to-know-info {
    background-color: white;
    text-align: center;
    padding: 40px;
    width: 220px;
    height: fit-content;
    margin-top: 80px;
    box-shadow: 10px 10px 25px rgba(0, 0, 0, 0.18);
}

.first-to-know-info h1 {
    font-size: 20pt;
}

.first-to-know-info p {
    font-size: 16pt;
}

.first-to-know-wrapper {
    background-image: url(./assets/images/front-page-first-to-know-mobile.png);
    background-size: cover;
    background-position: center;
}

/* applies on large screens. */
@media screen and (min-width: 1240px) {
    .launch-card-wrapper {
        flex-direction: row;
        width: 1000px;
        justify-content: space-between;
        margin: 0 auto;
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
        width: 1000px;
    }

    .hiring-section-wrapper {
        display: flex;
        justify-content: center;
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

    .first-to-know-wrapper {
        background-image: url(./assets/images/front-page-first-to-know.png);
        background-position: center;
        width: 100%;
        background-color: pink;
        display: flex;
        justify-content: center;
    }

    .first-to-know-content {
        display: flex;
        justify-content: flex-end;
        width: 1240px;
    }

    .first-to-know-info {
        margin-right: 60px;
    }

    .recruiter-wrapper {
        display: flex;
        justify-content: center;
        background-color: rgb(10, 32, 34);
        margin-top: 120px;
    }

    .recruiter-content {
        width: 1240px;
        margin-top: 0px;
    }

    .first-to-know-info {
        background-color: white;
        text-align: center;
        padding: 40px;
        padding-left: 20px;
        padding-right: 20px;
        width: 400px;
        height: fit-content;
    }

    .first-to-know-info h1 {
        font-size: 26pt;
    }

    .first-to-know-info p {
        font-size: 18pt;
    }

    .student-info-wrapper {
        display: flex;
        justify-content: space-between;
    }

    .student-info {
        width: 800px;
    }

    .student-info p:first-child {
        font-size: 20pt;
    }

    .student-info-wrapper-reverse {
        flex-direction: row-reverse;
    }
    .hired-on-handshake-img {
        width: 200px;
    }
}
</style>
