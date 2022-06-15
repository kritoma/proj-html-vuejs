<template>
  <section>
    <div class="container">
        <TitleSection title="Latest Band News"/>
    </div>
    <DisplayBar text="VIEW ALL LATEST NEWS"/>
  </section>
</template>

<script>
import DisplayBar from '../common/DisplayBar.vue';
import TitleSection from '../common/TitleSection.vue';

export default {
  components: { TitleSection, DisplayBar },
    name: "SectionBand"
}
</script>

<style lang="scss" scoped>
section{
    background-color: #252a33;
}
</style>