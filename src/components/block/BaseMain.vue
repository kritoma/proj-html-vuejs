<template>
  <main>
    <SectionMusicLife/>
    <SectionBand/>
    <SectionPlay/>
  </main>
</template>

<script>
import SectionBand from '../section/SectionBand.vue';
import SectionMusicLife from '../section/SectionMusicLife.vue';
import SectionPlay from '../section/SectionPlay.vue';

export default {
  components: { SectionMusicLife, SectionBand, SectionPlay },
    name: "BaseMain",
}
</script>

<style>

</style>