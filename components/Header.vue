<template>
<section class="container">
  <Header-bar/>
  <Side-bar/>
</section>
</template>

<script>
import HeaderBar from '~/components/HeaderBar.vue'
import SideBar from '~/components/SideBar.vue'

export default {
  components: {
    HeaderBar,
    SideBar
  }
}
function Addmin() {
  alert("sss");
};
</script>

<style lang="sass" scoped>
.container
  display: flex
</style>
