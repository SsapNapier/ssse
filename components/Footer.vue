<template>
<footer>
  <div class="contant">
    <div class="bottomBar">
      <h5>Адрес:</h5>
      <a href="#">г.Сочи, ул, Навагинская, д.14</a>
      <h5>Телефон:</h5>
      <a href="#">+7(862)264-45-55</a><br>
      <a href="#">+7(800)100-57-58</a>
      <h5>E-mail:</h5>
      <a href="#">info@aviatourne.ru</a>
    </div>
    <div class="bottomBar">
      <h5>Партнеры:</h5>
      <img src="./../assets/e-iata.png" class="main">
      <img src="./../assets/e-tkp@3x.png" class="main">
      <img src="./../assets/e-ural@3x.png" class="main">
    </div>
    <div class="bottomBar">
      <h5>Полезные ссылки</h5>
      <a href="#">Авиабилеты</a><br>
      <a href="#">Ж/Д билеты</a><br>
      <a href="#">Гостиницы</a><br>
      <a href="#">Трансфер</a><br>
      <a href="#">Партнерам</a><br>
    </div>
    <div class="bottomBar">
      <img src="./../assets/Path 308.svg" class="uni">
      <div class="items">
       <img src="#">
       <img src="./../assets/app-store.svg">
       <img src="./../assets/external-link.svg">
      </div>
       <i></i>
       <i></i>
       <p>Uniticket.aero – это продажа<br>
       билетов любых перевозчиков<br>
       сразу на все направления<br>
       в одном интерфейсе.</p>
      </div>
    <div class="bottomBar">
      <img src="./../assets/logo.svg" class="logo">
      <div class="items">
       <img src="#">
       <img src="#">
       <img src="./../assets/maps-and-flags.svg">
      </div>
      <br>
       <p>© АвиаТурне 2009 — 2019 <br> <br>
       Мы не штампуем - мы создаем<br>
       IT's WEB</p>
    </div>
  </div>
 </footer>
</template>

<script>
export default {
}
</script>

<style lang="sass" scoped>
@import '../assets/variables'
footer
  flex-wrap: wrap
  background-image: url(#)
  background-color: #1E1D1D
  // The backround color added to see better how will looks footer with background-img
  background-size: cover
  padding:
    top: $footer-padding-top
    bottom: $footer-padding-bottom
.contant
  display: flex
  font-family: SegoeUI
  width: $contant-width
  justify-content: space-between
  padding:
    left: $contant-left
.bottomBar
  display: flex
  flex-direction: column
  flex-shrink: 0
  margin-right: $bottom-margin-right
@media screen and (max-width: $adaptive-width)
  .contant
    padding:
      left: $adapt-contant-padding-left
      right: $adapt-contant-padding-right
@media screen and (max-width: $adaptive-width)
   .bottomBar
      margin-right: $adapt-bottom-r
.bottomBar h5
  color: white
  font-size: 14px
  font-weight: 600
  margin-bottom: 3%
.bottomBar a
  font-size: $adaptive-text
  line-height: 1.94
  color: $pinkish-grey
  outline: none
.bottomBar a:hover
  color: $azure
.bottomBar:nth-child(1) a
  padding:
    top: 4%
    bottom: 5%
.bottomBar:nth-child(3) a
  padding:
    top: 11%
.bottomBar p
  font-size: $adaptive-text
  color: $pinkish-grey
  line-height: 1.94
.bottomBar:nth-child(2) img
  position: relative
  top: 20px
  left: 0px
  padding:
    top: 7%
    bottom: 7%
.main
  max-width: 53px
.uni
  max-width: 27px
.items
  display: flex
  flex-direction: row
  justify-content: space-between
  max-width: 60%
  padding:
    top: 20%
    bottom: 16%
.logo
  max-width: 41px
</style>
