<template>
  <section>
    <div class="container">
        <TitleSection title="Music Is Life"/>
    </div>
  </section>
</template>

<script>
import TitleSection from '../common/TitleSection.vue';

export default {
  components: { TitleSection },
    name: "SectionMusicLife"
}
</script>

<style lang="scss" scoped>
section {
    background-color: #323844;
    padding: 1.875rem;
    position: relative;
    
    &::after {
        content: "";
        display: block;
        position: absolute;
        top: 0;
        left: 50%;
        transform: translateX(-50%);
        width: 400px;
        height: 10px;
        background-color: var(--color-primary);
    }

   
}
</style>