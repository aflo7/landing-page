<script setup></script>

<template>
    <div class="app-3-wrapper">
        <div class="app-3-content">
            <div class="hidden">
                <div class="handshake-logo-wrapper">
                    <img
                        src="../assets/images/logos/handshake.svg"
                        style="height: 40px"
                    />
                </div>
                <div class="store-icon-wrapper">
                    <img
                        src="../assets/images/apple-store.svg"
                        alt="apple-store-logo"
                        style="height: 30px; padding-right: 5px"
                    />

                    <img
                        src="../assets/images/google-play-store.svg"
                        alt="google-play-store-logo"
                        style="height: 30px; padding-left: 5px"
                    />
                </div>
            </div>

            <div class="flex-container">
                <div class="flex-item">
                    <div>
                        <div class="col-header">Students</div>
                        <div>How it works</div>
                        <div>Who's hiring</div>
                        <div>Career tips</div>
                        <div>Companies</div>
                        <div>Job roles</div>
                        <div>Help center</div>
                    </div>
                </div>
                <div class="flex-item">
                    <div>
                        <div class="col-header">Employers</div>
                        <div>Solutions</div>
                        <div>Products</div>
                        <div>Customers</div>
                        <div>Resources</div>
                        <div>Blog</div>
                        <div>Request demo</div>
                        <div>Help center</div>
                    </div>
                </div>

                <div class="flex-item">
                    <div>
                        <div class="col-header">Career Centers</div>
                        <div>Marketing toolkit</div>
                        <div>Resources</div>
                        <div>Events</div>
                        <div>Security</div>
                        <div>Request demo</div>
                        <div>Help center</div>
                    </div>
                </div>

                <div class="flex-item">
                    <div>
                        <div class="col-header">Company</div>
                        <div>About</div>
                        <div>Join us</div>
                        <div>Press</div>
                        <div>Blog</div>
                        <div>Brand guidelines</div>
                    </div>
                </div>

                <div class="flex-item">
                    <div>
                        <div class="col-header">Support</div>
                        <div>Students</div>
                        <div>Employers</div>
                        <div>Career enters</div>
                    </div>
                </div>

                <div class="flex-item icon-wrapper">
                    <div>
                        <div class="store-icon-wrapper">
                            <img
                                src="../assets/images/apple-store.svg"
                                alt="apple-store-logo"
                                style="width: 90px; padding-bottom: 15px;"
                            />

                            <img
                                src="../assets/images/google-play-store.svg"
                                alt="google-play-store-logo"
                                style="width: 90px;"
                            />
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div class="footer-wrapper">
        <footer>
            <div>
                <div>Privacy policy</div>
                <div>Terms of service</div>
                <div>Accessibility</div>
            </div>
            <div>©2023 <strong>Handshake</strong>. All rights reserved.</div>
        </footer>
    </div>
</template>

<style scoped>
.app-3-wrapper {
    background-color: rgb(245, 245, 247);
}

.footer-wrapper {
    background-color: rgb(245, 245, 247);
}
.flex-container {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    padding-top: 60px;
    padding-bottom: 60px;
    row-gap: 40px;
    font-size: 10pt;
}

.flex-item {
    width: 50%;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.flex-item > div {
    width: 100px;
}

.flex-item > div > div {
    cursor: pointer;
}
.flex-item > div > div:hover {
    /* width: 100px; */
    color: rgb(144, 78, 238);
}

.flex-item > div > div {
    padding-bottom: 15px;
}

.col-header {
    font-weight: bold;
    margin-top: 0px !important;
    padding-bottom: 25px;
}

.hidden {
    display: none;
}

.handshake-logo-wrapper {
    padding-top: 15px;
    padding-bottom: 40px;
    display: flex;
    justify-content: center;
}

.store-icon-wrapper {
    display: flex;
    flex-direction: column;
}

footer {
    font-size: 10pt;
    padding-bottom: 20px;
}

footer div:nth-child(1) {
    display: flex;
    justify-content: center;
}

footer div:nth-child(2) {
    text-align: center;
    padding: 5px;
}

footer div:nth-child(1) div {
    padding: 10px;
    cursor: pointer;
}

footer div:nth-child(1) div:hover {
    color: rgb(144, 78, 238);
}

@media screen and (min-width: 800px) {
    .flex-item {
        width: 33.3333%;
    }

    .app-3-content {
        padding-top: 40px;
    }
}

@media screen and (min-width: 1240px) {
    .flex-container {
        flex-grow: 1;
    }

    .flex-item {
        width: calc(100% / 6);
    }

    .hidden {
        padding-top: 30px;
        padding-right: 40px;
        display: block;
    }

    .app-3-wrapper {
        display: flex;
        justify-content: center;
    }

    .app-3-content {
        width: 1240px;
        display: flex;
        justify-content: space-between;
        padding-left: 40px;
        padding-bottom: 40px;
    }

    .icon-wrapper {
        display: none;
    }

    .col-header {
        padding-bottom: 40px;
    }

    .footer-wrapper {
        display: flex;
        justify-content: center;
    }

    footer {
        width: 1240px;
        border-top: 1px solid black;
        display: flex;
        padding-top: 10px;
    }

    footer div:nth-child(1) {
        order: 2;
    }

    footer div:nth-child(2) {
        order: 1;
    }

    footer div:nth-child(1) div {
        padding: 5px;
        margin-left: 10px;
    }

    .store-icon-wrapper {
    display: flex;
    flex-direction: row;
    justify-content: center;
}
}
</style>
