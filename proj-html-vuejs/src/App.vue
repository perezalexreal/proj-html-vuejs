<template>
  <div id="app">
<header-box :nav="nav" :logoPath="logoPath"/>
<jumbotron-box/>
  </div>
</template>

<script>
import HeaderBox from './components/HeaderBox.vue'
import JumbotronBox from './components/JumbotronBox.vue'


export default {
  name: 'App',
  components: {
    HeaderBox,
    JumbotronBox
  },
  data () {
    return {
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
@import './style/main.scss'

</style>
