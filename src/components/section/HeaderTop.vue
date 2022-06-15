<template>
  <div class="header_top">
    <LogoMusic/>
    <HamburgerMenu/>
  </div>
</template>

<script>
import HamburgerMenu from '../common/HamburgerMenu.vue';
import LogoMusic from '../common/LogoMusic.vue';

export default {
  components: { LogoMusic, HamburgerMenu },
    name: "HeaderTop"
}
</script>

<style lang="scss" scoped>
.header_top {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 1.25rem 3rem;
}

</style>