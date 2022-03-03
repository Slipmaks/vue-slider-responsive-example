<template>
  <h1>Slider</h1>
  <Splide :options="options">
    <SplideSlide>
      <img src="../img/blank-banner-lg-ex.png" alt="" />
    </SplideSlide>
    <SplideSlide>
      <img src="../img/blank-banner-lg-ex.png" alt="" />
    </SplideSlide>
    <SplideSlide>
      <img src="../img/blank-banner-lg-ex.png" alt="" />
    </SplideSlide>
  </Splide>
</template>
<script>
import "@splidejs/splide/dist/css/splide.min.css";
import { Splide, SplideSlide } from "@splidejs/vue-splide";

export default {
  components: {
    Splide,
    SplideSlide,
  },
  setup() {
    const options = {
      rewind: true,
      gap: "1rem",
      autoplay: true,
      speed: 3000,
      arrows: false,
      pagination: false,
    };

    return { options };
  },
};
</script>
