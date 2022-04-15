<script>
export default {};
</script>
<template>
  <section>
    <div class="max__w">
      <div class="flex flex-col items-center">
        <div class="text__Div">
          <h1>
            We are a trusted technology partner for
            <span>recognized brands</span>
          </h1>
          <h3>
            We give you exact quote before starting your project, and we stick
            to it! We give you exact quote before starting your project, and we
            stick to it!
          </h3>
        </div>
      </div>
      <div class="slider-container">
        <div class="slider-content-wrapper">
          <div class="slider-inner flex">
            <div class="slide">
              <img src="../img/wal.png" alt="wal" />
              <img class="two__logo" src="../img/wal.png" alt="wal" />
            </div>
            <div class="slide">
              <img src="../img/mic.png" alt="mic" />
              <img class="two__logo" src="../img/mic.png" alt="mic" />
            </div>
            <div class="slide">
              <img src="../img/hub.png" alt="hub" />
              <img class="two__logo" src="../img/hub.png" alt="hub" />
            </div>
            <div class="slide">
              <img src="../img/air.png" alt="air" />
              <img class="two__logo" src="../img/air.png" alt="air" />
            </div>
            <div class="slide">
              <img src="../img/wal.png" alt="wal" />
              <img class="two__logo" src="../img/wal.png" alt="wal" />
            </div>
            <div class="slide">
              <img src="../img/hub.png" alt="hub" />
            </div>
          </div>
        </div>
      </div>
      <!-- <div class="grid__logo__box">
        <div>
          <img src="../img/wal.png" alt="wal" />
          <img class="two__logo" src="../img/wal.png" alt="wal" />
        </div>
        <div>
          <img src="../img/mic.png" alt="mic" />
          <img class="two__logo" src="../img/mic.png" alt="mic" />
        </div>
        <div>
          <img src="../img/hub.png" alt="hub" />
          <img class="two__logo" src="../img/hub.png" alt="hub" />
        </div>
        <div>
          <img src="../img/air.png" alt="air" />
          <img class="two__logo" src="../img/air.png" alt="air" />
        </div>
        <div>
          <img src="../img/wal.png" alt="wal" />
          <img class="two__logo" src="../img/wal.png" alt="wal" />
        </div>
        <div>
          <img src="../img/hub.png" alt="hub" />
        </div>
      </div> -->
    </div>
  </section>
</template>
<style>
.grid__logo__box {
  margin-top: 60px;
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  gap: 50px;
}
.text__Div {
  margin-top: 100px;
  display: flex;
  justify-content: space-between;
  align-items: end;
}
.text__Div h1 {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 600;
  font-size: 37px;
  line-height: 49px;
  color: #2d3331;
}
.text__Div h1 span {
  color: #3db079ff;
}
.text__Div h3 {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 300;
  font-size: 17px;
  line-height: 23px;
  color: #b4b4b4;
  width: 782px;
  margin-left: 38px;
}
.two__logo {
  margin-top: 30px;
}

/* infinite Slider Go */
.slider-container {
  overflow: hidden;
  white-space: nowrap;
  margin-top: 90px;
  /* font-size: 0; */
}

.slider-content-wrapper {
  display: inline-block;
  white-space: nowrap;
  overflow: hidden;
  -webkit-animation: slide 20s linear infinite;
  animation: slide 20s linear infinite;
}

.slider-inner {
  white-space: nowrap;
  overflow: hidden;
  display: inline-block;
  /* margin-right: -5px; */
}

.slider-inner:last-child {
  margin-right: 0;
  display: flex;
}

.slide {
  /* display: inline-block; */
  display: flex;
  flex-direction: column;
  padding: 0 2.2rem;
  vertical-align: middle;
  outline: none;
  cursor: default;
  -webkit-transition: ease;
  transition: ease;
  margin-right: -5px;
}
.slide img {
  max-width: initial;
}

@keyframes slide {
  0% {
    -webkit-transform: translate3d(0, 0, 0);
    -moz-transform: translate3d(0, 0, 0);
    -ms-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
  }
  100% {
    -webkit-transform: translate3d(-50%, 0, 0);
    -moz-transform: translate3d(-50%, 0, 0);
    -ms-transform: translate3d(-50%, 0, 0);
    transform: translate3d(-50%, 0, 0);
  }
}

/* infinite Slider  Pause*/

@media (max-width: 1265px) {
  .grid__logo__box {
    margin-top: 60px;
    grid-template-columns: repeat(5, 1fr);
    gap: 30px;
  }
}

@media (max-width: 1138px) {
  .text__Div h1 {
    font-size: 32px;
    line-height: 40px;
  }
  .text__Div h3 {
    font-size: 15px;
    line-height: 25px;
    width: 650px;
    margin-left: 20px;
  }
  .grid__logo__box {
    margin-top: 50px;
    grid-template-columns: repeat(4, 1fr);
  }
}
@media (max-width: 813px) {
  .grid__logo__box {
    grid-template-columns: repeat(3, 1fr);
    gap: 30px;
  }
}
@media (max-width: 657px) {
  .grid__logo__box {
    grid-template-columns: repeat(2, 1fr);
    gap: 30px;
  }
}

@media (max-width: 1038px) {
  .text__Div h1 {
    font-size: 28px;
    line-height: 35px;
  }
  .text__Div h3 {
    font-size: 15px;
    line-height: 20px;
    width: 600px;
    margin-left: 20px;
  }
}
@media (max-width: 958px) {
  .text__Div {
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .text__Div h1 {
    text-align: center;
  }
  .text__Div h3 {
    margin-top: 10px;
    text-align: center;
    width: initial;
    margin-left: 0px;
  }
}
@media (max-width: 550px) {
  .text__Div {
    margin-top: 50px;
  }
  .text__Div h1 {
    font-size: 25px;
    line-height: 30px;
  }
  .text__Div h3 {
    font-size: 13px;
    line-height: 20px;
  }
}
@media (max-width: 438px) {
  .grid__logo__box {
    margin-top: 30px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
}
@media (max-width: 393px) {
  .text__Div h1 {
    font-size: 18px;
    line-height: 25px;
  }
  .text__Div h3 {
    font-size: 11px;
    line-height: 18px;
  }
}
</style>