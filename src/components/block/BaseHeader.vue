<template>
  <header>
    <HeaderTop/>
    <ContentHeader/>
  </header>
</template>

<script>
import ContentHeader from '../section/ContentHeader.vue';
import HeaderTop from '../section/HeaderTop.vue';

export default {
  components: { HeaderTop, ContentHeader },
    name: "BaseHeader",
}
</script>

<style lang="scss" scoped>
header {
    background-image: url("../../assets/img/home_slider.jpg");
    height: 100vh;
}
</style>