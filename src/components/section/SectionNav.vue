<template>
  <section>
    <div class="logo">
        <img src="../../assets/img/logo_footer.png" alt="logo">
    </div>
    <nav>
        <ul>
            <li v-for="(nav, index) in navs" :key="index"><a :href="nav.link">{{nav.name}}</a></li>
        </ul>
    </nav>
  </section>
</template>

<script>


export default {
    name: "SectionNav",
    data() {
        return {
            navs: [
                {
                    name: "Home",
                    link: "#"
                },
                {
                    name: "Meet The Band",
                    link: "#"
                },
                {
                    name: "Live Dates",
                    link: "#"
                },
                {
                    name: "Latest News",
                    link: "#"
                },
                {
                    name: "Albums",
                    link: "#"
                },
                {
                    name: "Fans",
                    link: "#"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
section{
    background-color: #323844;
    padding: 2rem;
    display: flex;
    justify-content: space-between;
    align-items: center;

    nav {
        ul {
            list-style: none;
            display: flex;
            gap: 1.25rem;
            margin: 0;

            a {
                text-decoration: none;
                color: #797d86;

                &:hover {
                    color: white;
                }
            }
        }
    }
    
}
</style>