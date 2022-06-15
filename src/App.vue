<template>
  <div id="app">
    <BaseHeader/>
    <BaseMain/>
    <BaseFooter/>
  </div>
</template>

<script>
import BaseFooter from './components/block/BaseFooter.vue';
import BaseHeader from './components/block/BaseHeader.vue';
import BaseMain from './components/block/BaseMain.vue';

export default {
  name: 'App',
  components: {
    BaseHeader,
    BaseMain,
    BaseFooter
  }
}
</script>

<style lang="scss">

</style>
