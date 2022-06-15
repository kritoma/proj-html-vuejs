<template>
  <div>
    <h2>{{title}}</h2>
    <hr>
    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ex, reiciendis quisquam? Quibusdam explicabo, reprehenderit impedit aspernatur saepe eligendi dicta neque repellendus deserunt, officiis nesciunt officia accusamus facere veritatis facilis eveniet.</p>
  </div>
</template>

<script>
export default {
    name: "TitleSection",
    props: {
        title: String
    }
}
</script>

<style lang="scss" scoped>
div{
    text-align: center;
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
</style>