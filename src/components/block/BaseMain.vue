<template>
  <main>
    <SectionMusicLife/>
    <SectionBand/>
  </main>
</template>

<script>
import SectionBand from '../section/SectionBand.vue';
import SectionMusicLife from '../section/SectionMusicLife.vue';

export default {
  components: { SectionMusicLife, SectionBand },
    name: "BaseMain",
}
</script>

<style>

</style>