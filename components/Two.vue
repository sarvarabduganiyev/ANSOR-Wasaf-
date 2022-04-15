<script>
export default {};
</script>

<template>
  <section class="max__w">
    <div>
      <div>
        <h1 class="our__services">Our services</h1>
      </div>
      <div class="gridCards__box">
        <div class="card__style card1">
          <div class="box__img">
            <img src="../img/card/1.png" alt="card1" />
          </div>
          <h1 class="__qator2">Dedicated team</h1>
          <h4 class="__qator2">
            We can make aweasome websites and Apps.We can make aweasome websites
            ....
          </h4>
        </div>
        <div class="card__style card1">
          <div class="box__img">
            <img src="../img/card/2.png" alt="card2" />
          </div>
          <h1 class="__qator2">Development of mobile applications</h1>
          <h4 class="__qator2">
            We can make aweasome websites and Apps.We can make aweasome websites
            ....
          </h4>
        </div>
        <div class="card__style card1">
          <div class="box__img">
            <img src="../img/card/3.png" alt="card3" />
          </div>
          <h1 class="__qator2">
            Development and implementation of ERP systems
          </h1>
          <h4 class="__qator2">
            We can make aweasome websites and Apps.We can make aweasome websites
            ....
          </h4>
        </div>
        <div class="card__style card1">
          <div class="box__img">
            <img src="../img/card/4.png" alt="card4" />
          </div>
          <h1 class="__qator2">UX/UI design</h1>
          <h4 class="__qator2">
            We can make aweasome websites and Apps.We can make aweasome websites
            ....
          </h4>
        </div>
        <div class="card__style card1">
          <div class="box__img">
            <img src="../img/card/5.png" alt="card5" />
          </div>
          <h1 class="__qator2">Infrastructure optimization</h1>
          <h4 class="__qator2">
            We can make aweasome websites and Apps.We can make aweasome websites
            ....
          </h4>
        </div>
        <div class="card__style card1">
          <div class="box__img">
            <img src="../img/card/6.png" alt="card6" />
          </div>
          <h1 class="__qator2">IT consulting</h1>
          <h4 class="__qator2">
            We can make aweasome websites and Apps.We can make aweasome websites
            ....
          </h4>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>

.gridCards__box {
  display: grid;
  grid-template-columns: calc(33.3% - 8px) calc(33.3% - 8px) calc(33.3% - 8px);
  gap: 24px;
}
.card__style {
  border: 1px solid #e8e8e8;
  border-radius: 16px;
  height: 232px;
}
.card1 {
  padding: 20px 32px;
}
.card1 .box__img {
  background: #e9faf2;
  border-radius: 8px;
  padding: 8px;
  display: inline-block;
}
.our__services {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 600;
  font-size: 35px;
  line-height: 160%;
  color: #2d3331;
}
.card__style h1 {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 700;
  font-size: 22px;
  line-height: 32px;
  color: #3db079;
}

.card__style h4 {
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  line-height: 24px;
  color: #969998;
}
@media (max-width: 1094px) {
  .gridCards__box {
    grid-template-columns: repeat(2, 1fr);
  }
  .card__style {
    height: initial;
  }
}
@media (max-width: 800px) {
  .card__style h1 {
    font-weight: 700;
    font-size: 20px;
    line-height: 30px;
  }
  .card__style {
    height: initial;
  }
  @media (max-width: 682px) {
    .card__style h1 {
      font-weight: 700;
      font-size: 18px;
      line-height: 30px;
    }
    .card__style h4 {
      font-size: 14px;
      line-height: 20px;
    }
  }
}
@media (max-width: 644px) {
  .gridCards__box {
    grid-template-columns: repeat(1, 1fr);
    gap: 12px;
  }
  .our__services {
    text-align: center;
  }
}
@media (max-width: 504px) {
  .card1 {
    padding: 15px 20px;
  }
  .our__services {
    font-weight: 600;
    font-size: 25px;
    line-height: 160%;
    color: #2d3331;
  }
  .max__w {
    max-width: 1300px;
    margin: 0 auto;
    padding: 0px 30px;
  }
  .card__style h1 {
    font-weight: 700;
    font-size: 18px;
    line-height: 23px;
  }
  .card__style h4 {
    font-size: 12px;
    line-height: 20px;
  }
}
</style>