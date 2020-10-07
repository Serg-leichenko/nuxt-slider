<template>
  <div class="header">
    <div class="header_content">
      <div class="logo">
        <a href="#">LOGO</a>
      </div>
      <div class="block-rigth">
        <div class="lang">
          <a href="#" class="fr">fr.</a>
          <a href="#" class="en">en.</a>
        </div>
        <div class="burger">
          <span></span>
          <span></span>
          <span></span>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.header_content {
  display: flex;
  justify-content: space-between;
  font-family: 'Montserrat', sans-serif;
}
.logo a {
  font-style: normal;
  font-weight: 800;
  font-size: 25px;
  letter-spacing: 4px;
  text-transform: uppercase;
}
.block-rigth {
  display: flex;
}
.lang a {
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  text-align: right;
  text-transform: uppercase;
}
.lang a:hover {
  opacity: 0.4;
}
.lang a:last-child {
  margin: 0 70px 0 40px;
}
.burger {
  cursor: pointer;
}
.burger span {
  display: block;
  width: 50px;
  height: 2px;
  background-color: #fff;
  margin-bottom: 6px;
}
a {
  text-decoration: none;
  color: #FFFFFF;
}
@media screen and (max-width: 480px){
  .lang {
    display: none;
  }
}
</style>