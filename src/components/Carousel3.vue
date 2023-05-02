<template>
    <div class="embla" ref="emblaNode">
        <div
            class="embla__container"
            style="display: flex; flex-direction: column; height: 150px"
        >
            <div class="embla__slide">
                <img
                    src="../assets/images/logos/general-mills.svg"
                    alt="gmills"
                    class="carousel-svg"
                />
            </div>
            <div class="embla__slide">
                <img
                    src="../assets/images/logos/us-house-of-representatives.png"
                    alt="us-house"
                    class="carousel-svg"
                />
            </div>
        </div>
    </div>
</template>

<script>
import emblaCarouselVue from "embla-carousel-vue"
import Autoplay from "embla-carousel-autoplay"

export default {
    name: "Carousel3",

    setup() {
        const [emblaNode] = emblaCarouselVue({ loop: true, axis: "y" }, [
            Autoplay({ delay: 6000 })
        ])
        return { emblaNode }
    }
}
</script>

<style scoped>
.embla {
    overflow: hidden;
}
.embla__container {
    display: flex;
}
.embla__slide {
    flex: 0 0 100%;
    min-width: 0;
}

.carousel-svg {
    height: 150px;
}
</style>
