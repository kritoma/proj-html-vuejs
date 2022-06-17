<template>
  <div class="content_header">
    <h1>Untold Stories</h1>
    <p>There is an untold story behind every favorite song.</p>
    <div class="buttons">
        <button class="btn_album">LATEST ALBUM</button>
        <button class="btn_live">LIVE DATES</button>
    </div>
  </div>
</template>

<script>
export default {
    name: "ContentHeader"
}
</script>

<style lang="scss" scoped>
.content_header {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: calc(100% - 115px);
    color: white;
    gap: 1.875rem;

    h1 {
        font-size: 6rem;
        font-weight: 700;
    }

    .buttons {
        display: flex;
        gap: .9375rem;

        button {
            padding: .5rem 1.25rem;
            color: white;
            background-color: inherit;
            border: .0625rem solid white;
        }

        .btn_album {
            background-color: var(--color-primary);
            border-color: var(--color-primary);
        }

        .btn_live:hover {
            background-color: white;
            color: black;
        }
    }
}
</style>