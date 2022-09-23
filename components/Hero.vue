<template>
  <div class="d-flex">
    <div id="hero-text">
      <h5>LUXURY GREEN & SMART HOMES</h5>
      <h1 id="transparent-text">
        FIND YOUR <br />
        NEXT HOME
      </h1>
      <button>Explore Our Properties</button>
    </div>
    <div id="heroImg">
      <img id="hero-img" src="../assets/hero-img.png" />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="css" scoped>
* {
  color: #b3b356;
}

#hero-text {
  padding: 100px 100px;
  background-image: url("assets/hero-text-bg.png");
}

#transparent-text {
  font-size: 80px;
  background: url("assets/hero-text-img.png") -20px -20px no-repeat;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  display: block;
  font-family: arial;
  font-weight: bold;
  background-size: cover;
}

#heroImg {
  display: flex;
  justify-content: center;
  align-items: center;
}
#hero-img {
  width: 600px;
  height: 590px;
  margin: 0 50px;
}

button {
  background-color: #b3b356;
  color: white;
  border: none;
  padding: 5px;
  font-weight: bold;
}
</style>
