<script>
export default {};
</script>
<template>
  <section class="max__w">
    <div>
      <div>
        <h1 class="text-center about__">About Our team</h1>
        <h3 class="text-center we__Are">
          We are a very experienced web & mobile app development team We are a
          very experienced web & mobile app development team
        </h3>
      </div>
      <div class="grid__Box">
        <div>
          <div class="relative imgBox">
            <img
              class="absolute w-full h-full object-cover"
              src="../img/person.png"
              alt="car"
            />
          </div>
          <div class="text__Box">
            <h1>Muhammad Xalil</h1>
            <h2>CEO</h2>
          </div>
        </div>
        <div>
          <div class="relative imgBox">
            <img
              class="absolute w-full h-full object-cover"
              src="../img/person.png"
              alt="car"
            />
          </div>
          <div class="text__Box">
            <h1>Muhammad Xalil</h1>
            <h2>CEO</h2>
          </div>
        </div>
        <div>
          <div class="relative imgBox">
            <img
              class="absolute w-full h-full object-cover"
              src="../img/person.png"
              alt="car"
            />
          </div>
          <div class="text__Box">
            <h1>Muhammad Xalil</h1>
            <h2>CEO</h2>
          </div>
        </div>
        <div>
          <div class="relative imgBox">
            <img
              class="absolute w-full h-full object-cover"
              src="../img/person.png"
              alt="car"
            />
          </div>
          <div class="text__Box">
            <h1>Muhammad Xalil</h1>
            <h2>CEO</h2>
          </div>
        </div>
        <div>
          <div class="relative imgBox">
            <img
              class="absolute w-full h-full object-cover"
              src="../img/person.png"
              alt="car"
            />
          </div>
          <div class="text__Box">
            <h1>Muhammad Xalil</h1>
            <h2>CEO</h2>
          </div>
        </div>
      </div>
      <div class="flex flex-col justify-center items-center">
        <div class="flex img__box justify-center items-center">
          <img class="play___img" src="../img/play.png" alt="play" />
          <img class="arrow___img" src="../img/arrow.png" alt="arrow" />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.grid__Box {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  gap: 15px;
  margin-top: 40px;
}
.imgBox {
  height: 280px;
}
.play___img {
    cursor: pointer;
}
.arrow___img {
  /* margin-left: 18px; */
  margin: 40px 0px 0px 18px;
}
.imgBox img {
  border-radius: 16px;
}
.text__Box h1 {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 600;
  font-size: 20px;
  line-height: 120%;
  color: #3db079;
  margin-top: 6px;
}
.text__Box h2 {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 300;
  font-size: 20px;
  line-height: 120%;
  color: #b4b4b4;
}
.about__ {
  margin-top: 100px;
  font-family: "Rubik";
  font-style: normal;
  font-weight: 600;
  font-size: 40px;
  line-height: 160%;
  color: #2d3331;
}
.we__Are {
  padding: 0px 250px;
  font-family: "Rubik";
  font-style: normal;
  font-weight: 300;
  font-size: 20px;
  line-height: 160%;
  text-align: center;
  color: #969998;
}

@media (max-width: 1200px) {
  .grid__Box {
    grid-template-columns: repeat(4, 1fr);
  }
}
@media (max-width: 1175px) {
  .we__Are {
    padding: 0px 150px;
  }
}

@media (max-width: 978px) {
  .grid__Box {
    grid-template-columns: repeat(3, 1fr);
  }
  .we__Are {
    padding: 0px 100px;
  }
}
@media (max-width: 820px) {
  .we__Are {
    padding: 0px 50px;
  }
}
@media (max-width: 754px) {
  .grid__Box {
    grid-template-columns: repeat(2, 1fr);
  }
}
@media (max-width: 643px) {
  .we__Are {
    padding: 0px;
  }
}
@media (max-width: 555px) {
  .about__ {
    font-size: 30px;
    line-height: 160%;
    margin-top: 50px;
  }

  .we__Are {
    font-size: 18px;
    line-height: 160%;
  }
}

@media (max-width: 450px) {
  .grid__Box {
    grid-template-columns: repeat(1, 1fr);
  }
}
@media (max-width: 555px) {
  .about__ {
    font-size: 27px;
    line-height: 160%;
  }
  .we__Are {
    font-size: 15px;
    line-height: 160%;
  }
}
</style>