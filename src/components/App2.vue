<script setup></script>

<template>
    <div class="pick-up-wrapper">
        <div class="pick-up-content">
            <img
                src="../assets/images/handshake-logo.png"
                alt="handshake-app-logo"
                class="handshake-app-logo"
            />

            <div class="pick-up-your-phone">Pick up your phone</div>

            <p style="font-size: 16pt">
                ... and never miss a message,<br />
                event, or job
            </p>

            <div class="download-wrapper">
                <img
                    src="../assets/images/apple-store.svg"
                    alt="apple-store-logo"
                    style="height: 60px; padding-right: 5px"
                />

                <img
                    src="../assets/images/google-play-store.svg"
                    alt="google-play-store-logo"
                    style="height: 60px; padding-left: 5px"
                />
            </div>
        </div>
        <div class="iphone-img-wrapper-mobile">
            <img src="../assets/images/front-page-phone.png" alt="iphone" />
        </div>

        <div class="iphone-img-wrapper-desktop">
            <img src="../assets/images/front-page-phone.png" alt="iphone" />
        </div>
    </div>

    <div class="find-wrapper">
        <div class="find-heading">
            Find the right jobs for you. <br />Get hired.
        </div>

        <div style="margin-top: 20px; width: 460px; display: flex">
            <input
                type="text"
                placeholder="Type .edu email here"
                class="edu-input"
                style="flex-grow: 1"
            />
            <button class="sign-up-btn">Sign up</button>
        </div>
    </div>
</template>

<style scoped>
.pick-up-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: rgb(113, 241, 253);
    text-align: center;
}

.download-wrapper {
    margin-top: 40px;
    margin-bottom: 40px;
}

.iphone-img-wrapper-mobile {
    margin-top: 20px;
    height: 340px;
    width: 100%;
    display: flex;
    justify-content: flex-end;
}

.iphone-img-wrapper-mobile img {
    width: 500px;
    height: auto;
}

.find-wrapper {
    background-color: rgb(10, 32, 34);
    color: white;
    text-align: center;
    padding-top: 200px;
    padding-bottom: 200px;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.sign-up-btn {
    border-radius: 5px;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
    font-size: 14pt;
    background-color: rgb(206, 249, 91);
    color: black;
}

.edu-input {
    padding: 10px;
    border-radius: 5px;
    border: none;
    margin-right: 15px;
}

.find-heading {
    font-size: 20pt;
    padding-bottom: 10px;
    font-weight: bold;
}

.iphone-img-wrapper-desktop {
    display: none;
}

.pick-up-your-phone {
    font-size: 50pt;
    font-family: "sansplomb";
    padding: 30px;
}

.handshake-app-logo {
    height: 120px;
    margin-top: 40px;
}

@media screen and (min-width: 1240px) {

  .find-heading {

  }
    .pick-up-wrapper {
        display: flex;
        flex-direction: row;
        justify-content: flex-end;
        position: relative;
        padding-top: 140px;
    }

    .pick-up-your-phone {
        padding: 0px;
    font-size: 70pt;

    }

    .pick-up-content {
        width: 1240px;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        text-align: left;
        padding-left: 40px;
    }

    .iphone-img-wrapper-mobile {
        display: none;
    }
    .iphone-img-wrapper-desktop {
        display: block;
    }

    .iphone-img-wrapper-desktop img {
        height: 440px;
    }
}
</style>
