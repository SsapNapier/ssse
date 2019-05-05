<template>
<header class="header-bar">

  <nuxt-link onclick="active(event)" to="/" class="header-bar_link active">Главная</nuxt-link>
  <nuxt-link onclick="active(event)" to="/okompanii" class="header-bar_link">О компании</nuxt-link>
  <nuxt-link onclick="active(event)" to="#" class="header-bar_link">Стать субагентом</nuxt-link>
  <nuxt-link onclick="active(event)" to="#" class="header-bar_link">Услуги</nuxt-link>
  <nuxt-link onclick="active(event)" to="#" class="header-bar_link">Контакты</nuxt-link>

   <script type="text/javascript">
    function active(event){
      var target = event.target;
      var i = 0;
      var link = document.getElementsByClassName('header-bar_link');
      link[0].classList.remove('active');
      link[1].classList.remove('active');
      link[2].classList.remove('active');
      link[3].classList.remove('active');
      link[4].classList.remove('active');
      target.classList.add('active');
     }
     // I don't know why, but method "for" don't work here.
     // Work on how to replace script in external file,
     // or, even better, how to make it with vue.js and place it in "<script>"
   </script>

 </header>
</template>

<script>

</script>

<style lang="sass" scoped>
@import '../assets/variables'
.header-bar
  position: relative
  top: $headbar-top
  width: $headbar-width
  display: flex
  height: $headbar-height
  justify-content: space-between
  margin-right: $space-menu
  &:before
    margin-top: $line-top
    content: ""
    display: inline-block
    vertical-align: middle
    width: $line-width
    min-width: $line-min-width
    height: 1px
    background: $pinkish-grey
    margin-right: $line-space
@media screen and (max-width: $adaptive-width)
  .header-bar
    width: $adaptive-headerbar-width
    margin-right: $adapt-space-menu
    &:before
      width: $adaptive-line-width
      min-width: 0
.header-bar_link
  font-family: SegoeUI
  font-size: $text-size
  color: $pinkish-grey
  cursor: pointer
  text-decoration: none
  margin-right: $links-indent
  outline: none
  flex-shrink: 0
  &:hover
    color: $azure
    border-bottom: 1px solid $azure
    text-decoration: none
  &.active
    color: $azure
    border-bottom: 1px solid $azure
.header-bar_link:nth-child(5)
      margin-right: $last-link
@media screen and (max-width: $adaptive-width)
  .header-bar_link
    font-size: $adaptive-text
</style>
