<template>
  <div>
    <div id="card-container">
      <nuxt-link to="products/lands">
        <div class="card">
          <div>
            <img src="../../assets/land.svg" alt="" srcset="" />
            <h1>Land</h1>
          </div>
        </div></nuxt-link
      >
      <div class="card">
        <div>
          <img src="../../assets/homes.png" alt="" srcset="" />
          <h1>Homes</h1>
        </div>
      </div>
      <div class="card">
        <div>
          <img src="../../assets/investment.svg" alt="" srcset="" />
          <h1>Investments</h1>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="css" scoped>
* {
  text-decoration: none;
}

a {
  text-decoration: none;
  color: white;
}
#card-container {
  display: flex;
  justify-content: space-around;
  margin: auto;
}
.card {
  background: #00367c;
  color: white;
  height: 500px;
  width: 300px;
  margin: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  border-radius: 10px;
  transition: transform ease-in-out 0.5s;
  cursor: pointer;
  box-shadow: 0px -1px 20px 2px rgb(0 0 0 / 31%);
}

.card:hover {
  transform: scale(1.1);
}

.card img {
  margin: 30px;
}
</style>
