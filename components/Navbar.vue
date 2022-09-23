<template>
  <nav ref="navRef">
    <img src="../assets/gtexthomes-logo.png" />
    <div class="d-flex">
      <ul v-for="(link, index) in links" :key="index">
        <li id="nav-list">
          <nuxt-link :to="link.path">{{ link.name }}</nuxt-link>
        </li>
      </ul>
    </div>
    <button></button>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      links: [
        {
          name: "Home",
          path: "/",
          component: "pages/index.vue",
        },
        {
          name: "Products",
          path: "/products",
          component: "pages/products.vue",
        },
        {
          name: "Visit us",
          path: "/",
          component: "pages/visit-us.vue",
        },
        {
          name: "About us",
          path: "/about",
          component: "pages/about-us.vue",
        },
      ],
    };
  },

  // methods: {
  //   onScroll() {
  //     let prev = window.scrollY;
  //     const refs = this.$refs.navRef;
  //     window.addEventListener("scroll", () => {
  //       var curr = window.scrollY;
  //       if (prev > curr) {
  //         refs.classList.add("scroll");
  //         refs.classList.remove("scrolledDown");
  //         console.log(curr);
  //       } else {
  //         refs.classList.add("scrolledDown");
  //         refs.classList.remove("scroll");
  //       }
  //       if (curr === 0) {
  //         refs.classList.remove("scroll");
  //         refs.classList.remove("scrolledDown");
  //       }
  //     });
  //   },
  // },

  // mounted() {
  //   this.onScroll();
  //   console.log("mounted");
  // },
};
</script>

<style lang="css" scoped>
nav {
  position: fixed;
  left: 0;
  top: 0;
  z-index: 200;
  background: white;
  width: 100vw;
  height: 120px;
  text-decoration: none;
  list-style-type: none;
  display: flex;
  justify-content: space-around;
  align-items: center;
  box-shadow: 2px 3px 10px 0px #00000021;
}

img {
  width: 40px;
  height: 50px;
}

li {
  list-style-type: none;
}

a {
  color: rgb(0, 0, 0);
  text-transform: uppercase;
  text-decoration: none;
  letter-spacing: 0.15em;
  display: inline-block;
  padding: 15px 20px;
  position: relative;
}

a:after {
  background: none repeat scroll 0 0 transparent;
  bottom: 0;
  content: "";
  display: block;
  height: 2px;
  left: 50%;
  position: absolute;
  background: rgb(237, 10, 10);
  transition: width 0.3s ease 0s, left 0.3s ease 0s;
  width: 0;
}

a:hover:after {
  width: 100%;
  left: 0;
}

button {
  background-color: red;
  color: white;
  width: 60px;
}
</style>
