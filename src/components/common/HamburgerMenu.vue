<template>
  <div class="hambuger_menu">
    <i @click="openMenu()" class="fa-solid fa-bars"></i>
    <div v-show="isOpen" class="open_menu" >
      <div class="top_menu">
        <img src="../../assets/img/avada-music-logo.png" alt="logo">
        <i @click="closeMenu()" class="fa-solid fa-xmark"></i>
      </div>
      <nav>
        <ul>
          <li v-for="(nav, index) in navs" :key="index"><a :href="nav.link">{{nav.name}}</a></li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
    name: "HamburgerMenu",
    data() {
        return {
            isOpen: false,
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
    },

    methods: {
      openMenu() {
        this.isOpen = true
      },

      closeMenu() {
        this.isOpen = false
      }
    }
}
</script>

<style lang="scss" scoped>
.hambuger_menu {
    color: white;

    i {
        font-size: 2rem;
    }

    .open_menu {
      width: 100vw;
      height: 100vh;
      background-color: var(--color-primary);
      color: #f78f99;
      z-index: 10;
      position: absolute;
      top: 0;
      left: 0;
      
      

      .top_menu {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1.25rem 3rem;

        i {
          margin-right: 25px;
        }
      }

      nav {
        text-align: center;
        

        ul {
          display: flex;
          flex-direction: column;
          align-items: center;
          list-style: none;
          gap: 1.5rem;
          

          a {
            text-decoration: none;
            color: #f78f99;
            font-size: 40px;

            &:hover {
              color: white;
            }
          }
        }
      }
    }
}
</style>