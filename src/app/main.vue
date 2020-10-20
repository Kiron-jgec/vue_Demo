<template>
  <div class="main">
    <!-- header Section -->

  
      <header>
        <nav>
          <a href="#" data-aos="fade-right" data-aos-duration="2000"> <img src="../assets/logos/long_logo.svg" alt="" /></a>
          <div class="headerSec" data-aos="fade-right" data-aos-duration="2000">
            <span> HOME </span>
            <span> CARERRS </span>
            <span> CONTACT </span>
            <span> LOGIN </span>
            <span @click="showhideLoader" > {{loaderText}} </span>

          </div>
        </nav>
      </header>




    <!-- fast video Section  -->
  
      <div class="videoContainer">
        <div class="videoSec">
          <video class="vid-bg" autoplay loop>
            <source src="../assets/videos/video1.mp4" type="video/mp4" />
          </video>
        </div>

        <div class="mainTestsec">
          <h1 data-aos="zoom-out" data-aos-duration="3000">Let’s create something amazing together.</h1>

          <button data-aos="fade-up"
     data-aos-duration="3000">Get Start</button>
        </div>



      </div>

     
   

    <!-- aim section  -->
    <div class="textHerSe" data-aos="fade-right" data-aos-duration="3000">
      <h1>The future of logistics, delivered today.</h1>
      <p>
        We’re developing the next generation of logistics technology, to help
        the world move things faster and smarter than ever before.
      </p>
    </div>

    <section>
      <div class="aimSec" >
        <div class="aimContainer" data-aos="fade-right" data-aos-duration="3000">
          <h1 >What do we do?</h1>
          <p>
            As most BI tools provide you tools that a BI specialist can utilize
            for their data analytics, we let your data tell YOU what is
            important.
          </p>
        </div>
      </div>
    </section>
 <loader v-if="loader"></loader>







    <!-- services section  -->

    <section>
      <div class="servicesSec">
        <div
          class="serviceContiner"
          v-for="(services, idx) in servicesData"
          :key="idx"
          data-aos="flip-left" data-aos-duration="2500"
        >
          <img :src="services.imgurl" alt="" />
          <hr />
          <h3>{{ services.text }}</h3>

          <p>{{ services.disCrip }}</p>
        </div>
      </div>
    </section>



    <!-- man with smile face  -->

    <section>
      <div class="mancontainer">
        <div class="imgSec" data-aos="zoom-in" data-aos-duration="3000">
          <img src="../assets/images/smilyMan.jpg" alt="" />
        </div>

        <div class="textSec"
         data-aos="fade-down"
         data-aos-duration="3000"
     >
          <h1>Request a demoHay this is Proper Section</h1>
          <p>
            Are you ready to Partner with us to get your desired Development
            Services for Android Apps, iPhone Apps, iPad Apps, Hybrid &amp;
            Native Apps, etc?
          </p>
        </div>
      </div>
    </section>

    <!-- motivate section  -->

    <section>
      <div class="motivate">
        <div class="motContainer" data-aos="zoom-out" data-aos-duration="3000">
          <h1>Everything around you has been moved.</h1>
          <p>
            Touching dozens of hands and traveling thousands of miles. On
            conveyor belts, planes, trailers, and trucks. To get to you, now.
            Yet, as technology continues to alter the ways we live, work, and
            play, logistics remains the same. We’re here to change that.
          </p>
        </div>
      </div>
    </section>

    <section>
      <div class="teamContainer">
        <div class="comtainertext" 

    data-aos="fade-down"
     data-aos-easing="linear"
     data-aos-duration="2500"
     >
          <h1>Get the most out of your data</h1>
          <p>
            Our easy-to-use smart dashboards will give you insights that will
            bring your business to the next level. Request a demo and experience
            the value for yourself.
          </p>

          <button>Start Now</button>
        </div>
      </div>
    </section>

    <!-- video Section 2   -->

    <section>
      <div class="videoContainer" data-aos="zoom-in"  data-aos-duration="3000">
        <div class="videoSec">
          <video class="vid-bg" autoplay loop>
            <source src="../assets/videos/video2.mp4" type="video/mp4" />
          </video>
        </div>
      </div>
    </section>

    <footer>
      <div class="footerSec">
        <div class="imgSecF" data-aos="fade-right" data-aos-duration="3000">
          <a href="#"> <img src="../assets/logos/long_logo.svg" alt="" /></a>
          <h3>Let’s create something amazing together.</h3>
        </div>
        <div class="linkSecF" data-aos="zoom-in" data-aos-duration="3000">
          <span> HOME </span>
          <span> CARERRS </span>
          <span> CONTACT </span>
          <span> LOGIN </span>
        </div>
        <div class="socialSec" data-aos="fade-up"
     data-aos-duration="3000">
          <h3>Join With Us</h3>
          <input type="email" />
          <button>Join</button><br /><br /><br />

          <a href="https://www.facebook.com/bymond"
            ><i class="fa fa-facebook-square" aria-hidden="true"></i>
          </a>

          <a href="https://www.youtube.com/channel/UCJyCEQkzS2mQ0GIt-xnJmzQ"
            ><i class="fa fa-youtube-play" aria-hidden="true"></i
          ></a>

          <a href="https://twitter.com/bymondofficial"
            ><i class="fa fa-twitter-square" aria-hidden="true"></i
          ></a>
          <a href="https://www.instagram.com/bymondofficial/"
            ><i class="fa fa-instagram" aria-hidden="true"></i
          ></a>

          <a href="https://www.linkedin.com/company/bymond/"
            ><i class="fa fa-linkedin-square" aria-hidden="true"></i
          ></a>
        </div>
      </div>

      <div class="copySec" data-aos="fade-right" data-aos-duration="3000">
        &#169; 2020 - All Rights Reserve - Developer : Injamamul Hoque
      </div>
    </footer>
  </div>
</template>

<script>
 import loader from "./loader"
export default {
  data() {
    return {

loader:false,
loaderText : "SHOW LOADER",

      servicesData: [
        {
          text: "No Expensive BI consultants",
          imgurl:
            "https://crebosbi.com/sites/default/files/2020-05/icons8-code-80%201%20%281%29.png",
          disCrip:
            "BI specialists are hard to find and expensive, let our smart dashboards do the complex work for you.",
        },

        {
          text: "No need for your own tech team",
          imgurl:
            "https://crebosbi.com/sites/default/files/2020-05/icons8-code-80%201%20%286%29.png",
          disCrip:
            "Easy-to-use dashboards, no need for your own IT specialists.",
        },

        {
          text: "Detailed profits information",
          imgurl:
            "https://crebosbi.com/sites/default/files/2020-05/icons8-code-80%201%20%287%29.png",
          disCrip:
            "Detailed KPI information like you have never seen before. Get everything out of your data.",
        },

        {
          text: "Fast implementation cycle",
          imgurl:
            "https://crebosbi.com/sites/default/files/2020-05/icons8-code-80%201%20%288%29.png",
          disCrip:
            "Short implementation time, from start to development, to launch.",
        },
      ],
    };
  },
  components:{
      loader
  },
  methods:{
showhideLoader()
{
    if(this.loader==false)
    {
        this.loader=true;
        this.loaderText= "HIDE LOADER" ;

    }
    else 
    {
        this.loader=false;
        this.loaderText= "SHOW LOADER" ;

    }
}

  }
};
</script>





<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@900&display=swap");








/* header Section  */

header {
  padding: 10px 20px;
  background: #00000067;
  position: fixed;
  width: 100%;
  z-index: 1;
}

nav {
  display: flex;

  align-items: center;
}
nav img {
  height: 35px;
}

.headerSec {
  width: fit-content;
  position: absolute;

  right: 50px;
  color: white;
  font-family: inherit;
}
.headerSec span {
  margin: 0px 5px;
  font-family: inherit;
  font-size: 13px;
  font-family: "Roboto", sans-serif;
  cursor: pointer;
  padding: 5px ;
  
}

.headerSec span:hover
{
    border-bottom: 2px #ff6200 solid;
}
/* fast video Section  */

.videoContainer {
  position: relative;
}
.videoSec {
  width: 100%;
  height: 100%;

  background: rgb(0, 0, 0);
}

.vid-bg {
  opacity: 0.6; /* ! */

  right: 0;
  bottom: 0;
  width: 100%;
  height: 100%;
}
.mainTestsec {
  position: absolute;

  top: 20%;
  padding: 20px 10%;
  text-align: center;
}
.mainTestsec h1 {
  color: white;
  font-family: "Roboto", sans-serif;
  font-size: 85px;
}

.mainTestsec button {
  padding: 20px 50px;
  margin: 20px 0px;
  outline: none;
  border-radius: 4px;
  border: none;
  font-family: "Roboto", sans-serif;
  font-size: 20px;
  background: #007bff;
  color: white;
  cursor: pointer;
  transition: 0.6s;
}
.mainTestsec button:hover {
  background: #ff6200f5;
}
/* ami section  */

.aimSec {
  width: 100%;
  height: 900px;
  position: relative;
  background-image: url("../assets/images/img1.png");
  background-repeat: no-repeat;
  background-size: 100%;
}
.textHerSe {
  padding: 5%;
  
}
.textHerSe {
  text-align: center;
}
.textHerSe h1 {
  color: #007bff;
  font-family: "Roboto", sans-serif;
  font-size: 45px;
}
.textHerSe p {
  color: #838383;
  font-family: "Roboto", sans-serif;
  font-size: 17px;
  margin: 10px 20%;
  width: 60%;
}
.aimContainer {
  position: absolute;
  top: 360px;
  right: 50px;
  width: 50%;
  padding: 20px;
}
.aimContainer h1 {
  color: #ffffff;
  font-family: "Roboto", sans-serif;
  font-size: 45px;
}
.aimContainer p {
  color: #ffffff;
  font-family: "Roboto", sans-serif;
  font-size: 22px;
}

/* services section */

.servicesSec {
  display: grid;

  grid-template-columns: repeat(auto-fit, minmax(15rem, 18rem));

  justify-content: center;
  align-items: center;
  grid-gap: 20px;
}
.serviceContiner {
  background: rgb(253, 253, 253);
  text-align: center;
  padding: 10px;
  overflow: hidden;
  border: 1px rgb(206, 206, 206) solid;

  border-radius: 4px;
  transition: transform 0.5s;
  cursor: pointer;
}
.serviceContiner:hover {
  box-shadow: 0px 8px 16px 0px rgba(43, 43, 43, 0.2);
  transform: translateY(-15px);
}
.serviceContiner hr {
  border: 3px solid #ff6200;
  border-radius: 5px;
  margin: 15px 0px;
  width: 30%;
}
.serviceContiner h3 {
  font-family: "Roboto", sans-serif;
  color: #007bff;
  margin: 7px 0px;
}
.serviceContiner p {
  font-family: "Roboto", sans-serif;
  color: #999999;
  margin: 7px 0px;
  text-align: left;
  font-size: 15px;
}

/* man with smaile face  */

.mancontainer {
  display: grid;
  width: 100%;
  grid-template-columns: repeat(auto-fit, minmax(15rem, 35rem));

  justify-content: center;
  align-items: center;
  grid-gap: 50px;
}
.imgSec {
  padding: 20px;
}
.imgSec img {
  width: 80%;
  border: 25px #ff6200f5 solid;
}

.textSec {
  padding: 15px;
}
.textSec h1 {
  font-family: "Roboto", sans-serif;
  color: #007bff;
  font-size: 40px;
}
.textSec p {
  font-family: "Roboto", sans-serif;
  color: #838383;
  font-size: 18px;
}

/* motivation section  */

.motivate {
  width: 100%;
  height: 900px;

  position: relative;
 
  background-image: url("../assets/images/transport.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: fixed;
  display: flex;
  text-align: center;
  align-items: center;
  justify-content: center;
}
.motContainer {
  padding: 15px;

  width: 80%;
}
.motContainer h1 {
  font-family: "Roboto", sans-serif;
  color: #ffffff;
  font-size: 50px;
  margin: 20px 0px;
}

.motContainer p {
  font-family: "Roboto", sans-serif;
  color: #ffffff;
  font-size: 20px;
  margin: 20px 0px;
}

/* more section  */

.teamContainer {
  width: 100%;
  height: 900px;
  position: relative;
  position: relative;
  background-image: url("../assets/images/img2.png");
  background-repeat: no-repeat;
  background-size: 100%;
  background-position: fixed;
}
.comtainertext {
  width: 40%;
  position: absolute;
  top: 300px;
  right: 25px;
}

.comtainertext h1 {
  font-family: "Roboto", sans-serif;

  font-size: 50px;
  color: #ff6200f5;
}
.comtainertext p {
  font-family: "Roboto", sans-serif;
  color: #838383;
  font-size: 18px;
  margin: 20px 0px;
}
.comtainertext button {
  padding: 15px 50px;
  margin: 10px 0px;
  outline: none;
  border-radius: 4px;
  border: none;
  font-family: "Roboto", sans-serif;
  font-size: 18px;
  background: #007bff;
  color: white;
  cursor: pointer;
  transition: 0.6s;
}
.comtainertext button:hover {
  background: #ff6200f5;
}

/* footer */

footer {
  background: #0b0d11f5;
  padding: 20px 10px;
}
.footerSec {
  display: grid;

  grid-template-columns: repeat(auto-fit, minmax(15rem, 25rem));

  justify-content: center;
  align-items: center;
  grid-gap: 30px;
}
.imgSecF,
.linkSecF,
.socialSec {
  padding: 10px;
  margin: 20px 0px;
}
.imgSecF img {
  width: 100%;
}
.imgSecF h3,
.socialSec h3 {
  font-family: "Roboto", sans-serif;
  color: white;
  margin: 10px 0px;
  font-size: 24px;
}
.linkSecF {
  text-align: center;
}
.linkSecF span {
  font-family: "Roboto", sans-serif;
  color: white;
  margin: 0px 5px;
  font-size: 13px;
  cursor: pointer;
  padding: 5px 0px;
}
.linkSecF span:hover {
  border-bottom: 2px #ff6200f5 solid;
}
.socialSec {
}
.socialSec input {
  width: 80%;
  padding: 8px 5px;
  outline: none;
  font-family: "Roboto", sans-serif;
}
.socialSec button {
  padding: 9px 15px;
  font-family: "Roboto", sans-serif;
  background: #ff6200f5;
  border: none;
  color: white;
  outline: none;
  cursor: pointer;
}
.socialSec a {
  background: rgb(255, 255, 255);
  padding: 15px;
  margin: 0px 5px;
  border-radius: 50%;
  color: #007bff;
  transition: 0.6s;
}
.socialSec a:hover {
  background: #ff6200f5;
  color: white;
}
.socialSec a i {
  font-size: 20px;
}

.copySec {
  width: 100%;
  text-align: center;
  margin: 30px 0px 0px 0px;
  color: rgb(151, 151, 151);
  font-family: "Roboto", sans-serif;
  font-size: 13px;
}

/* nagative Space  */

.textHerSe 
{
    margin: 5% 0px;
}
.servicesSec,.mancontainer,.motivate,.teamContainer
{
    margin: 20% 0px;

}





</style>