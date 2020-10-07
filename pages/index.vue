<template>
  <div class="container">
    <Header />
    <Slider />
  </div>
</template>

<script>
import Header from '@/components/Header';
import Slider from '@/components/Slider';
export default {
  components: {
    Header,
    Slider
  }
};
</script>

<style>
.container {
  background: #000;
  margin: 0 auto;
  min-height: 100vh;
  padding: 60px 70px 270px 70px;
}
@media screen and (max-width: 480px){
  .container {
    padding: 60px 30px 270px 30px;
  }
}
</style>
