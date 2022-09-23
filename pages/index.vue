<template>
  <div>
    <Hero />
    <section id="info-box">
      <div class="info box1">
        <div><h1>10</h1></div>
        <p>
          BRANCHES ALL OVER <br />
          <span class="info-span"> WORLD</span>
        </p>
      </div>
      <div class="info box2">
        <div><h1>15+</h1></div>
        <p>
          FULLY SERVICED <br /><span class="info-span">REGISTERED ESTATES</span>
        </p>
      </div>
      <div class="info box3">
        <div><h1>14+</h1></div>
        <p>YEARS OF <br /><span class="info-span">EXPERIENCE</span></p>
      </div>
      <div class="info box4">
        <div><h1>24</h1></div>
        <p>
          HOURS <br />
          <span class="info-span"> CUSTOMER SERVICE</span>
        </p>
      </div>
    </section>
    <section id="location">
      <div>
        <h2 class="title locations">
          <span class="span loc1">located in </span
          ><span class="span loc2"> three continents</span>
        </h2>
      </div>
      <div id="location-flag">
        <img src="../assets/nig.png" />
        <img src="../assets/uk.png" />
        <img src="../assets/dubia.png" />
      </div>
      <button class="btn read-more1">READ MORE</button>
    </section>
    <section id="slider1">
      <Slider />
    </section>
    <section id="core">
      <div>
        <h2 class="title core-value">
          <span class="span core-title1">CORE</span
          ><span class="span core-title2"> VALUES</span>
        </h2>
        <div class="core-values">
          <div class="core1">
            <img src="../assets/energy.svg" />
            <h2>ENERGY</h2>
            <p>
              Exhibiting positive energy by taking innitiative to make things
              happens.
            </p>
          </div>
          <div class="core1">
            <img src="../assets/excellence.svg" />
            <h2>EXCELLENCE</h2>
            <p>Doing ordinary things extraordinarily.</p>
          </div>
          <div class="core1">
            <img src="../assets/hand-shake.svg" />
            <h2>INTEGRITY</h2>
            <p>
              Doing the right things by maintaining the highest level of ethical
              standards without exceptions.
            </p>
          </div>
          <div class="core1">
            <img src="../assets/rocket.svg" />
            <h2>INNOVATION</h2>
            <p>
              Seeking new and better ways to produce result by being open minded
              and thinking differently.
            </p>
          </div>
        </div>

        <button class="btn read-more1">READ MORE</button>
      </div>
    </section>
    <section><Slider /></section>
    <section id="sac">
      <div><img src="../assets/SA-pic.png" /></div>
      <div style="padding: 50px">
        <h2>
          “Owning the land is what matters <br />
          the most; whoever owns the land <br />
          controls the cashflow.”
        </h2>
        <h5>-DR STEPHEN AKINTAYO</h5>
        <h6>(GMD/CEO, GTEXT HOLDINGS)</h6>
      </div>
    </section>
    <section id="partners">
      <h2 class="title partner">Partners</h2>
      <div class="pt-img">
        <div class="partner-img">
          <img src="../assets/gvest.png" alt="" srcset="" />
        </div>
        <div class="partner-img">
          <img src="../assets/SAC-logo.png" alt="" srcset="" />
        </div>
        <div class="partner-img">
          <img src="../assets/gvest.png" alt="" srcset="" />
        </div>
        <div class="partner-img">
          <img src="../assets/gtextacademy.svg" alt="" srcset="" />
        </div>
        <div class="partner-img">
          <img src="../assets/g&a.svg" alt="" srcset="" />
        </div>
        <div class="partner-img">
          <img src="../assets/gvest.png" alt="" srcset="" />
        </div>
        <div class="partner-img">
          <img src="../assets/gsoft.svg" alt="" srcset="" />
        </div>
        <div class="partner-img">
          <img src="../assets/gvest.png" alt="" srcset="" />
        </div>
      </div>
    </section>
    <section id="gvest">
      <h1>DOWNLOAD THE NEW GVEST APP</h1>
      <p>
        Lorem ipsum dolor sit amet. 33 voluptatem porro et incidunt galisum est
        optio internos id minus voluptatem! Et <br />
        minus molestiae hic quisquam praesentium nam impedit tempore in quia
        necessitatibus ut aliquam labore! Ut odio exercitationem et veniam quae
        et corrupti necessitatibus eum eaque sint est consequatur dolor quo
        nulla ipsa eum Quis Quis.
      </p>
      <button>
        <img src="../assets/download-gvest-button.png" alt="" />
      </button>
    </section>
    <div>
      <div id="sub">
        <h2>BE A PART OF OUR PROGRAMS</h2>
        <P
          >Be the first to get updates on our activities & exciting developments
          towards building a better future!</P
        >
        <button>SUBSCRIBE</button>
      </div>
      <div class="footer">
        <img src="../assets/white-logo.png" />
        <div class="foot">
          <div class="foot-in">
            <div class="footer-end">
              <p>309 Close, Banana Island, Ikoyi Lagos, Nigeria</p>
              <p>info@gtexthomes.com</p>
              
              <p>+234 704 839 8466</p>
              <p>+234 704 839 8466</p>
            </div>
            <div class="footer-end">
              <p>About</p>
              <p>About Gtext Homes</p>
              <p>Careers</p>
              <p>Privacy Policy</p>
            </div>
            <div class="footer-end">
              <p>Helpful Links</p>
              <p>Contact Us</p>
              <p>Blog</p>
              <p>Projects</p>
            </div>
            <div class="footer-end-last">
              <p>Follow Us</p>
              <img src="../" />
            </div>
          </div>
        </div>
        <div class="copyright">
          <img src="../assets/gsoft.png" alt="" srcset="" />
          <p style="color: white">
            2022 GtextSoft Software Solutions. All rights reserved. Gtext Homes
            is a brand of Gtext Holdings.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Hero from "../components/Hero.vue";
import Slider from "../components/Slider.vue";
export default {
  name: "IndexPage",
  components: { Hero, Slider },
};
</script>

<style>
.btn {
  border-radius: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: auto;
  padding: 5px 20px;
  letter-spacing: 4px;
}

.btn.read-more1 {
  border: 2px solid #b3b356;
  color: #b3b356;
}

.title {
  font-weight: 500;
  font-size: 60px;
  text-align: center;
  text-transform: uppercase;
  font-family: "Bebas Neue";
  width: 100vw;
  position: relative;
}
.title.locations::before {
  content: "OUR GLOBALIZATION PLAN";
  position: absolute;
  top: -30%;
  left: 40%;
  font-size: 20px;
  letter-spacing: 8px;
  color: #b3b356;
}
.span {
  font-weight: 500;
  font-size: 60px;
  text-align: center;
  text-transform: uppercase;
  font-family: "Bebas Neue";
  width: 100vw;
  position: relative;
}

.span.loc1 {
  color: #b3b356;
}

.span.loc2 {
  color: #ff0009;
}

.span.core-title1 {
  color: #b3b356;
}
.span.core-title2 {
  color: #00367c;
}

.title.core-value::before {
  content: "our";
  position: absolute;
  top: -30px;
  left: 48%;
  font-size: 20px;
  letter-spacing: 6px;
  color: #00367c;
}
.title.partner::before {
  content: "our";
  position: absolute;
  top: -30px;
  left: 48%;
  font-size: 20px;
  letter-spacing: 6px;
  color: #ff0009;
}
.title.partner {
  color: #00367c;
}

#info-box {
  display: grid;
  grid-template-columns: 1fr 1fr;
  column-gap: 50px;
  row-gap: 50px;
  padding: 70px 100px;
}

.info {
  height: 180px;
  border: 2px solid #dadadadf;
  display: flex;
  justify-content: center;
  align-items: center;
  box-shadow: 2px 3px 10px 0px #00000021;
}

.info h1,
.info p {
  color: #b3b356;
}

.info span {
  color: #ff0009;
}

.box1 {
  border-radius: 100px 0 0 0;
}

.box2 {
  border-radius: 0 100px 0 0;
}

.box3 {
  border-radius: 0 0 0 100px;
}

.box4 {
  border-radius: 0 0 100px 0;
}
#location {
  background-image: url("assets/location-bg.png");
  height: 500px;
  width: 100vw;
  padding: 20px 0;
}
#location-flag {
  display: flex;
  justify-content: center;
  align-items: center;
}
#location-flag img {
  margin: 50px 20px;
}

#slider1 {
  background-image: url("assets/slider-bg.png");
}

#core {
  padding-top: 90px;
}
#core img,
#core h2 {
  padding: 10px 0;
}

#core h2 {
  color: #00367c;
  font-family: "Bebas Neue", sans-serif;
}

#core p {
  color: #00367c;
}
.core-values {
  display: grid;
  grid-template-columns: 1fr 1fr;
  margin: auto;
}

.core1 {
  width: 600px;
  height: 360px;
  border: 1px solid #dadada;
  border-radius: 10px;
  margin: 20px;
  text-align: center;
  padding: 70px;
}

#sac {
  display: flex;
  justify-content: center;
  align-items: center;
}

#sac h2 {
  font-family: "Raleway";
  color: #00367c;
}
#sac h5 {
  color: #ff0009;
}
#sac h6 {
  color: #b3b356;
}

#partners {
  padding-top: 90px;
}
.partner-img {
  border: 1px solid #dadada;
  height: 140px;
  width: 275px;
  border-radius: 10px;
  margin: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.pt-img {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
}

#gvest {
  background: url("assets/download-gvest.png");
  padding: 120px 70px;
}

#gvest h1,
#gvest p {
  color: white;
  text-align: center;
  padding: 10px 0;
}

#gvest h1 {
  font-family: "Bebas Neue";
}

#gvest p {
  font-family: "Raleway";
}
#gvest button {
  border: none;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: auto;
  border-radius: 20px;
}

#sub {
  padding: 90px 70px;
  text-align: center;
}

#sub button {
  background: #ff0009;
  border: none;
  padding: 10px 20px;
  border-radius: 20px;
  color: white;
}

#sub h2 {
  font-family: "Bebas Neue";
}
.footer {
  background: #001127;
}
.foot {
  padding: 50px 50px 50px 90px;
}
.foot-in {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  border-bottom: 2px solid white;
  padding: 20px 0;
}
.footer-end {
  color: white;
  padding: 20px;
  border-right: 2px solid white;
}
.footer-end-last {
  color: white;
  padding: 20px;
}

.copyright {
  text-align: center;
}
</style>
