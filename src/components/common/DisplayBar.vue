<template>
  <div>
    <h5>{{text}}</h5>
  </div>
</template>

<script>
export default {
    name: "DisplayBar",
    props: {
        text: String,
    }
}
</script>

<style lang="scss" scoped>
div {
    background-color: var(--color-primary);
    padding: 40px 0;
    text-align: center;
    color: white;

    h5 {
        font-size: 14px;
        margin: 0;
    }
}
</style>