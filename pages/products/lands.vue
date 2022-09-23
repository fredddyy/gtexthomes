<template>
  <div id="header">
    <h1>
      Don’t wait to buy land,<br />
      buy land and wait
    </h1>
    <p>-Dr Stephen Akintayo</p>
    <div>
      <Cards />
    </div>
  </div>
</template>

<script>
import Cards from "../../components/Cards.vue";
export default {
  components: { Cards },
};
</script>

<style lang="css" scoped>
img {
  height: 200px;
  width: 100px;
}
#header {
  display: block;
  justify-content: center;
  align-items: center;
  margin: auto;
}

#header h1,
p {
  text-align: center;
}

#header p {
  color: #ff0009;
  font-size: 25px;
  font-weight: 300;
}
#header h1 {
  font-size: 50px;
  font-weight: bold;
}

#sub-title {
  color: #ff0009;
}
</style>
