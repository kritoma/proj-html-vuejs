<template>
  <section>
    <h2>Music Is Life</h2>
    <hr>
    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. A nostrum pariatur voluptatem earum quasi quia. Reiciendis autem asperiores sed laborum culpa sunt ipsa dolorem a cum reprehenderit? Ipsum, repudiandae omnis.</p>
  </section>
</template>

<script>
export default {
    name: "SectionMusicLife"
}
</script>

<style lang="scss" scoped>
section {
    background-color: #323844;
    text-align: center;
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

    h2 {
        color: white;
        font-size: 4rem;
    }

    hr {
        width: 15%;
        color: #444e62;
        height: 3px;
        margin: 1.25rem auto;
    }

    p {
        color: #7d7b8d;
        width: 50%;
        margin: auto;
    }
}
</style>