<template>
  <main>
    <SectionMusicLife/>
    <SectionBand/>
    <SectionPlay/>
    <SectionLiveDates/>
  </main>
</template>

<script>
import SectionBand from '../section/SectionBand.vue';
import SectionLiveDates from '../section/SectionLiveDates.vue';
import SectionMusicLife from '../section/SectionMusicLife.vue';
import SectionPlay from '../section/SectionPlay.vue';

export default {
  components: { SectionMusicLife, SectionBand, SectionPlay, SectionLiveDates },
    name: "BaseMain",
}
</script>

<style>

</style>