<template>
  <div class="slider">
    <div id="slide" v-for="i in [currentIndex]" :key="i">
      <div class="text">
        <img class="icon" src="../assets/next.svg" @click="next" />
        <img class="icon" src="../assets/prev.svg" @click="prev" />
        <p class="before">AFRICA’S LARGEST DEVELOPERS OF</p>
        <h1 id="title">GREEN & SMART HOMES</h1>
        <p>
          {{ current.text }}
        </p>
        <button>Read more</button>
      </div>
      <div>
        <div class="img-container">
          <img :src="current.img" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Slider",
  data() {
    return {
      content: [
        {
          img: require("../assets/slide-img1.png"),
          text: "We are the Africa’s largest developers of luxury green smart homes and as forefronters setting the pace in thisfield, we have a vision of building 25,000 housing unitsby the year 2035 and we seek to achieve this with themost advanced cutting-edge technology at our disposal.",
        },
        {
          img: "https://cdn.pixabay.com/photo/2016/02/17/23/03/usa-1206240_1280.jpg",
          text: "757875473",
        },
        {
          img: "https://cdn.pixabay.com/photo/2015/05/15/14/27/eiffel-tower-768501_1280.jpg",
          text: "34574352475",
        },
        {
          img: "https://cdn.pixabay.com/photo/2016/12/04/19/30/berlin-cathedral-1882397_1280.jpg",
          text: "retueht9eqio",
        },
      ],
      timer: null,
      currentIndex: 0,
    };
  },
  // mounted() {
  //   this.startSlide();
  // },
  methods: {
    startSlide: function () {
      this.timer = setInterval(this.next, 3000);
    },

    next: function () {
      this.currentIndex += 1;
    },

    prev: function () {
      this.currentIndex -= 1;
    },
  },

  computed: {
    current: function () {
      return this.content[Math.abs(this.currentIndex) % this.content.length];
    },
  },
};
</script>

<style lang="css" scoped>
@import url("https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap");
#slide {
  display: grid;
  grid-template-columns: 1fr 1fr;
  width: 100vw;
}

#title {
  font-family: "Bebas Neue";
  font-size: 60px;
  position: relative;
}

#title::after {
  content: url("assets/underline.png");
  position: absolute;
  top: 25px;
  left: 0;
  width: 20 px;
}
p {
  font-family: "Raleway", sans-serif;
}

p.before {
  letter-spacing: 5px;
}
.slider {
  display: grid;
  grid-template-columns: 1fr 1fr;
  justify-content: center;
  align-items: center;
  height: 700px;
  margin: 40px 0;
  background: url("assets/slider-bg.png");
  color: white;
}
.icon {
  height: 30px;
  width: 30px;
  border: 2px solid #dadada;
  border-radius: 50px;
  box-sizing: content-box;
  cursor: pointer;
}

.text {
  padding: 50px;
}
#trans {
  position: relative;
  width: 100%;
  height: 100%;
  padding: 100px;
}

img {
  width: 100%;
  height: 100%;
  border-radius: 0 80px 0 80px;
  margin: 40px;
}

/* .fade-enter-active,
.fade-leave-active {
  transition: all 0.9s ease;
  overflow: hidden;
  visibility: visible;
  position: absolute;
  opacity: 1;
  width: 100%;
  height: 100%;
}

.fade-enter,
.fade-leave-to {
  visibility: hidden;
  opacity: 0;
  position: absolute;
  width: 100%;
  height: 100%;
} */

.prev,
.next {
  cursor: pointer;
  width: auto;
  padding: 16px;
  color: black;
  font-weight: bold;
  font-size: 18px;
  transition: 0.7s ease;
  border-radius: 0 4px 4px 0;
  user-select: pointer;
}

.prev:hover,
.next:hover {
  background-color: rgba(0, 0, 0, 0.9);
}

.img-container {
  width: 400px;
  height: 430px;
  position: relative;
}

.img-container::before {
  content: url("assets/dubia.png");
  position: absolute;
  top: -5px;
  border-radius: 50%;
  border: 15px solid blue;
}

@keyframes tonext {
  75% {
    left: 0;
  }
  95% {
    left: 100%;
  }
  98% {
    left: 100%;
  }
  99% {
    left: 0;
  }
}

@keyframes tostart {
  75% {
    left: 0;
  }
  95% {
    left: -300%;
  }
  98% {
    left: -300%;
  }
  99% {
    left: 0;
  }
}

@keyframes snap {
  96% {
    scroll-snap-align: center;
  }
  97% {
    scroll-snap-align: none;
  }
  99% {
    scroll-snap-align: none;
  }
  100% {
    scroll-snap-align: center;
  }
}
</style>
