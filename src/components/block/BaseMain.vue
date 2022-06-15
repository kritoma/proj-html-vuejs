<template>
  <main>
    <SectionMusicLife/>
    <SectionBand/>
    <SectionPlay/>
    <SectionLiveDates/>
    <SectionNav/>
  </main>
</template>

<script>
import SectionBand from '../section/SectionBand.vue';
import SectionLiveDates from '../section/SectionLiveDates.vue';
import SectionMusicLife from '../section/SectionMusicLife.vue';
import SectionNav from '../section/SectionNav.vue';
import SectionPlay from '../section/SectionPlay.vue';

export default {
  components: { SectionMusicLife, SectionBand, SectionPlay, SectionLiveDates, SectionNav },
    name: "BaseMain",
}
</script>

<style>

</style>