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

<style scoped>
img {
  width: 100%;
  height: 100%;
  padding-right: 80px;
}
.social-block {
  width: 30px;
  margin-top: 50px;
  font-family: "Montserrat", sans-serif;
}
.social a {
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  text-align: right;
  text-transform: uppercase;
  color: #fff;
  text-decoration: none;
  transform: rotate(-90deg);
  display: block;
}
.social a:nth-child(2) {
  margin: 50px 0;
}
.slider-text {
  position: absolute;
  color: #fff;
  top: 40%;
  z-index: 1;
}
.subtitle {
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  text-transform: uppercase;
  color: #a3a3a3;
  mix-blend-mode: normal;
  opacity: 0.5;
}
.title {
  font-family: "Barlow Condensed", sans-serif;
  font-style: normal;
  font-weight: 900;
  font-size: 100px;
  text-transform: uppercase;
  color: #ffffff;
}
@media screen and (max-width: 732px){
  .title {
    font-size: 70px;
  }
}
@media screen and (max-width: 480px){
  img {
    padding-right: 5px;
  }
  .slider-text {
    top: 33%;
  }
  .social-block {
    display: none;
  }
}
@media screen and (max-width: 442px) {
  .title {
    font-size: 50px;
  }
}
</style>
