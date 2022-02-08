<template>
  <div id="app">
<header-box :nav="nav" :logoPath="logoPath"/>
  </div>
</template>

<script>
import HeaderBox from './components/HeaderBox.vue'


export default {
  name: 'App',
  components: {
    HeaderBox
  },
  data () {
    return {
      logoPath: '../assets/logo-sidearea-1-1.png',
      nav : [
        'Home',
        'Pages',
        'Portfolio',
        'Blog',
        'Shop',
        'Elements',
      ],
    }
  }
}
</script>

<style lang="scss">

</style>
