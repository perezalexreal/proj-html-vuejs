<template>
  <div id="app">
    <header-box :nav="nav" :logoPath="logoPath" />
    <jumbotron-box />
    <section-images />
    <section-working />
    <section-contact/>
    <section-blog/>
    <footer-box/>
  </div>
</template>

<script>
import HeaderBox from "./components/HeaderBox.vue";
import JumbotronBox from "./components/JumbotronBox.vue";
import SectionImages from "./components/SectionImages.vue";
import SectionWorking from "./components/SectionWorking.vue";
import SectionContact from "./components/SectionContact.vue";
import SectionBlog from "./components/SectionBlog.vue";
import FooterBox from "./components/FooterBox.vue";


export default {
  name: "App",
  components: {
    HeaderBox,
    JumbotronBox,
    SectionImages,
    SectionWorking,
    SectionContact,
    SectionBlog,
    FooterBox
  },
  data() {
    // Array utilizzato in HeaderBox attraverso i props
    return {
      nav: ["Home", "Pages", "Portfolio", "Blog", "Shop", "Elements"],
    };
  },
};
</script>

<style lang="scss">
@import "./style/main.scss";
</style>
