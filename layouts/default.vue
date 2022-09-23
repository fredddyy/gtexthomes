<template>
  <div>
    <Navbar />
    <Nuxt id="body" />
  </div>
</template>

<script>
import Navbar from "../components/Navbar.vue";
export default {
  components: { Navbar },
};
</script>

<style lang="css">
@import url("https://fonts.googleapis.com/css2?family=Josefin+Sans:wght@100;200;300;400;500;600;700&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Raleway:wght@200;300;400;500;600;700&display=swap");

* {
  font-family: "Josefin Sans", sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
}

#body {
  margin-top: 130px;
}
</style>
