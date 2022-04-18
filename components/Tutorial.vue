<script>
export default {
  data() {
    return {
      toggleWord: false,
    };
  },
  methods: {
    toggle() {
      this.toggleWord = !this.toggleWord;
      if (this.toggleWord) {
        document.querySelector("body").style.overflow = "hidden";
      } else {
        document.querySelector("body").style.overflow = "initial";
      }
    },
  },
};
</script>
<template>
  <div>
    <div class="bg__green">
      <div>
        <nav
          class="
            max__w
            navbar__div
            relative
            z-10
            flex
            justify-between
            items-center
            text-white
          "
        >
          <div class="logo_box">
            <img src="../img/a__logo.png" alt="nav__logo" />
          </div>
          <div
            :style="[toggleWord ? { left: '0' } : { left: '-100%' }]"
            class="navbar__links flex items-center"
          >
            <ul class="ul__links flex items-center">
              <li><a class="nav__links links__1" href="#">About</a></li>
              <li><a class="nav__links links__2" href="#">Portfolio</a></li>
              <li><a class="nav__links links__3" href="#">Our services</a></li>
              <li><a class="nav__links links__4" href="#">Contact</a></li>
            </ul>
            <div class="contact__btn__box">
              <button>Contact</button>
            </div>
          </div>
          <div class="burger__div">
            <button @click="toggle" class="burger__btn" v-if="toggleWord">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="h-6 w-6 text-white"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
                stroke-width="2"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M6 18L18 6M6 6l12 12"
                />
              </svg>
            </button>
            <button @click="toggle" v-else class="burger__btn">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="h-6 w-6 text-white"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
                stroke-width="2"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M4 6h16M4 12h16M4 18h16"
                />
              </svg>
            </button>
          </div>
        </nav>
      </div>
      <!-- .scroll__btn,#container,.texts__box{
    z-index: -1;
  } -->
      <div
        :style="[toggleWord ? { zIndex: '-5' } : { zIndex: '5' }]"
        class="texts__box max__w relative z-10"
      >
        <h1 class="text-center">We want to work with you</h1>
        <p class="text-center">
          We are a very experienced web & mobile app development team
        </p>
      </div>
      <div
        id="container"
        :style="[toggleWord ? { zIndex: '-5' } : { zIndex: '5' }]"
        class="max__w relative z-10"
      >
        <div class="item">
          <h1 class="inline-block lets__talk">LET’S TALK</h1>
        </div>
        <div class="circle aylana1"></div>
        <div class="circle aylana2"></div>
        <div class="circle aylana3"></div>
        <div class="circle aylana4"></div>
      </div>
      <div
        :style="[toggleWord ? { zIndex: '-5' } : { zIndex: '5' }]"
        class="
          scroll__btn
          max__w
          relative
          z-10
          flex flex-col
          animate-bounce
          items-end
          justify-center
          bottom-20
        "
      >
        <img src="../img/scroll.png" alt="scroll" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.bg__green {
  background-image: url("../img/stars.gif");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 700px;
  position: relative;
}
.bg__green:after {
  background-color: #163828;
  position: absolute;
  width: 100%;
  height: 100%;
  content: "";
  top: 0;
  left: 0;
  opacity: 0.7;
}
.navbar__div {
  height: 80px;
}
.nav__links {
  font-family: "Poppins";
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  line-height: 20px;
}
.links__2,
.links__3,
.links__4 {
  margin-left: 38px;
}
.contact__btn__box button {
  margin-left: 70px;
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 20px;
  padding: 9px 40px;
  background: #3db079;
  border: 1px solid #3db079;
  border-radius: 8px;
  transition: 0.3s ease;
}
.contact__btn__box button:hover {
  background: #fff;
  color: #3db079;
}
.texts__box {
  margin-top: 130px;
}
.texts__box h1 {
  font-family: "Comfortaa";
  font-style: normal;
  font-weight: 700;
  font-size: 60px;
  line-height: 70px;
  background: linear-gradient(180deg, #ffffff 48.65%, #193b2b 80.72%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

#container {
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  margin-top: 100px;
}
.ping__box {
  margin-top: 20px;
}
.texts__box p {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 30px;
  text-align: center;
  color: #c0ddcf;
  padding: 0px 320px;
}
.lets__talk {
  width: 120px;
  height: 120px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  border-radius: 50%;
  font-family: "Comfortaa";
  font-style: normal;
  font-weight: 700;
  font-size: 15px;
  background-color: #fff;
  line-height: 20px;
  text-align: center;
  color: #133224;
}
.burger__div {
  display: none;
}
.circle {
  border-radius: 50%;
  background-color: transparent;
  border: 1px solid #fff;
  width: 10px;
  height: 10px;
  position: absolute;
  opacity: 1;
}

.aylana1 {
  animation: scaleIn 2.3s infinite;
  animation-delay: 2.5s;
}

.aylana2 {
  animation: scaleIn 2.3s infinite;
  animation-delay: 3s;
}

.aylana3 {
  animation: scaleIn 2.3s infinite;
  animation-delay: 3.5s;
}

.aylana4 {
  animation: scaleIn 2.3s infinite;
  animation-delay: 4s;
}

@keyframes scaleIn {
  from {
    padding: 2px;
    opacity: 0.5;
  }

  to {
    padding: 100px;
    opacity: 0;
  }
}

@media (max-width: 1161px) {
  .texts__box p {
    padding: 0px 200px;
  }
}
@media (max-width: 1000px) {
  .texts__box p {
    font-size: 18px;
    line-height: 30px;
    padding: 0px 100px;
  }
  #container {
    margin-top: 150px;
  }
  .links__2,
  .links__3,
  .links__4 {
    margin-left: 20px;
  }
  .contact__btn__box button {
    margin-left: 40px;
  }
  .texts__box h1 {
    font-size: 50px;
    line-height: 60px;
  }
}
@media (max-width: 869px) {
  .navbar__links {
    position: fixed;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: #000;
    opacity: 0.7;
    color: white;
    transition: 0.3s ease;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    z-index: 1px;
  }
  .ul__links {
    flex-direction: column;
  }
  .links__1 {
    font-size: 19px;
    line-height: 35px;
  }
  .links__2,
  .links__3,
  .links__4 {
    margin-left: 0px;
    margin-top: 20px;
    font-size: 19px;
    line-height: 35px;
  }
  .contact__btn__box button {
    margin-left: 0px;
    font-size: 19px;
    line-height: 35px;
    /* margin-top: 20px; */
    padding: initial;
    background: initial;
    border: none;
    border-radius: 0px;
    transition: initial;
  }
  .contact__btn__box button:hover {
    background: initial;
    color: initial;
  }
  .burger__div {
    display: block;
  }
  .burger__div,
  .logo_box {
    z-index: 70;
  }
  /* .scroll__btn,#container,.texts__box{
    z-index: -1;
  } */
}
@media (max-width: 785px) {
  .texts__box p {
    font-size: 15px;
    line-height: 25px;
    padding: 0px 30px;
  }
  .texts__box h1 {
    font-size: 40px;
    line-height: 50px;
  }
}
@media (max-width: 550px) {
  .logo_box img {
    width: 150px;
  }
}
@media (max-width: 435px) {
  .texts__box p {
    font-size: 14px;
    line-height: 22px;
    padding: 0px;
  }
  .texts__box h1 {
    font-size: 30px;
    line-height: 40px;
  }
}
@media (max-width: 367px) {
  .logo_box img {
    width: 120px;
  }
}
</style>