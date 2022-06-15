<template>
  <div class="cardDates">
    <i class="fa-solid fa-plus"></i>
    <p>{{live.date}}, {{live.festival}}, {{live.country}}</p>
  </div>
</template>

<script>
export default {
    name: "CardDates",
    props: {
        live: Object,
    }
}
</script>

<style lang="scss" scoped>
.cardDates {
    background-color: #323844;
    color: var(--color-primary);
    display: flex;
    align-items: center;
    gap: 1.25rem;
    padding: 10px;

    p {
        margin: 0;
    }

    i {
        color: white;
        font-size: 8px;
        margin-left: 1.25rem;
    }
}
</style>