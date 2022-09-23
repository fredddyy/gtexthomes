<template>
  <div>
    <div id="cards">
      <div class="container" v-for="props in lands">
        <div id="card">
          <img id="prop-img" :src="require(`/assets/` + props.imgUrl)" />
          <h3>{{ props.name }}</h3>
          <div class="d-flex">
            <h4>ISHERI</h4>
          </div>
          <div class="d-flex">
            <div id="box">
              <h6>N15M</h6>
              <h6>OUTRIGHT</h6>
            </div>
            <div id="box">
              <h6>N15M</h6>
              <h6>OUTRIGHT</h6>
            </div>
            <div id="box">
              <h6>N15M</h6>
              <h6>OUTRIGHT</h6>
            </div>
          </div>
          <img id="img-feat" src="../assets/estate-feautures.png" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      lands: [
        { name: 1, imgUrl: "jasper-smart-city.png" },
        { name: 2, imgUrl: "jasper-smart-city.png" },
        { name: 3, imgUrl: "jasper-smart-city.png" },
        { name: 4, imgUrl: "jasper-smart-city.png" },
        { name: 4, imgUrl: "jasper-smart-city.png" },
        { name: 4, imgUrl: "jasper-smart-city.png" },
      ],
    };
  },

  mounted() {
    console.log(this.lands);
  },
};
</script>

<style lang="css" scoped>
#card {
  padding: 10px;
  width: 350px;
  background-color: white;
  border-radius: 20px;
  box-shadow: 2px 4px 16px 6px rgb(0 0 0 / 13%);
}

#prop-img {
  height: 350px;
  width: 350px;
  border: blue;
}
#img-feat {
  width: 330px;
  height: 45px;
}
#map-pin {
  height: 20px;
  width: 20px;
}
#box {
  background-color: #dadada;
  border-radius: 5px;
  height: 50px;
  width: 80px;
  margin: 4px;
}
#cards {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  row-gap: 50px;
  column-gap: 50px;
  margin: auto;
}
</style>
