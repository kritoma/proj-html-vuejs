<template>
  <section>
    <div class="container">
        <p>"I just listened to it and said to myself, "Man, I really love this album." Still, today, it just sounds so fresh. It sounds full of ideas. These guys knew what they were doing. They're good. And they're inventive. I haven't heard anything this year that's as inventive. i don't really expect to."</p>
        <i class="fa-solid fa-play"></i>
    </div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
section {
    background-image: url("../../assets/img/home-testimonial-parallax.jpg");
    background-size: cover;
    background-position: center;
    padding: 100px 0;
    color: white;
    text-align: center;

    .container {
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    
    p {
        width: 50%;
    }

    i{
        display: flex;
        align-items: center;
        justify-content: center;
        width: 50px;
        height: 50px;
        border-radius: 50%;
        background-color: var(--color-primary);
    }
}
</style>