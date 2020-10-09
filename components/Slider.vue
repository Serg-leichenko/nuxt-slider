<template>
  <div>
    <div class="slider-text">
      <div class="subtitle">design</div>
      <div class="title">Red BLACK</div>
    </div>
    <hooper :settings="hooperSettings">
      <slide>
        <img src="../images/image1.jpg" />
      </slide>
      <slide>
        <img src="../images/image2.jpg" />
      </slide>
      <slide>
        <img src="../images/image1.jpg" />
      </slide>
      <slide>
        <img src="../images/image2.jpg" />
      </slide>

      <hooper-navigation slot="hooper-addons"></hooper-navigation>
    </hooper>
    <div class="social-block">
      <div class="social">
        <a href="#" class="fr">fb</a>
        <a href="#" class="en">be</a>
        <a href="#" class="Inst">Inst</a>
      </div>
    </div>
  </div>
</template>

<script>
import { Hooper, Slide, Navigation as HooperNavigation } from "hooper";
import "hooper/dist/hooper.css";

export default {
  components: {
    Hooper,
    Slide,
    HooperNavigation,
  },
  data() {
    return {
      hooperSettings: {
        itemsToShow: 1.25,
        itemsToSlide: 1,
        centerMode: true
      }
    };
  },
};
</script>