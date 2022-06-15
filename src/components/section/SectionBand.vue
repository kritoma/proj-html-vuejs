<template>
  <section>
    <div class="container">
        <TitleSection title="Latest Band News"/>
    </div>
  </section>
</template>

<script>
import TitleSection from '../common/TitleSection.vue'
export default {
  components: { TitleSection },
    name: "SectionBand"
}
</script>

<style lang="scss" scoped>
section{
    background-color: #252a33;
}
</style>