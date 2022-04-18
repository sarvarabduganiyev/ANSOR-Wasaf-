<script>
export default {};
</script>
<template>
  <section id="portfolio">
    <div class="max__w">
      <div class="texts__div">
        <h1>Our portfolio</h1>
        <h2>
          We give you exact quote before starting your project, and we stick to
          it!
        </h2>
      </div>
      <div>
        <div class="Grid__content">
          <div class="grid__items items1">
            <div>
              <img src="../img/air1.png" alt="air" />
            </div>
            <div><h1>We give you exact quote before startin</h1></div>
          </div>
          <div class="grid__items items2">
            <div
              class="grid__items__big flex flex-col justify-center items-center"
            >
              <div>
                <img src="../img/hub1.png" alt="hub1" />
              </div>
              <div><h1>We give you exact quote before startin</h1></div>
            </div>
          </div>
          <div class="grid__items items3">
            <div>
              <img src="../img/air1.png" alt="air" />
            </div>
            <div><h1>We give you exact quote before startin</h1></div>
          </div>
          <div class="grid__items items4">
            <div>
              <img src="../img/mic1.png" alt="mic1" />
            </div>
            <div><h1>We give you exact quote before startin</h1></div>
          </div>
          <div class="grid__items items5">
            <div>
              <img src="../img/wal1.png" alt="wal1" />
            </div>
            <div><h1>We give you exact quote before startin</h1></div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>


<style scoped>
.texts__div {
  margin-top: 120px;
}
.texts__div h1 {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 600;
  font-size: 40px;
  line-height: 50px;
  text-align: center;
  color: #2d3331;
}
.texts__div h2 {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 24px;
  text-align: center;
  color: #b4b4b4;
}

.Grid__content {
  margin-top: 40px;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(2, 1fr);
  gap: 20px;
}

.items1 {
  grid-area: 1 / 1 / 2 / 2;
  background: #f7575c;
  border-radius: 16px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 70px 30px;
}
.items2 {
  grid-area: 1 / 2 / 3 / 3;
  background: #ee721c;
  border-radius: 16px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 70px 30px;
}
.items3 {
  grid-area: 2 / 3 / 3 / 4;
  background: #3db079;
  border-radius: 16px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 70px 30px;
}
.items4 {
  grid-area: 1 / 3 / 2 / 4;
  background: #00a3ee;
  border-radius: 16px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 70px 30px;
}
.items5 {
  grid-area: 2 / 1 / 3 / 2;
  background: #f7ae2e;
  border-radius: 16px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 70px 30px;
}
.grid__items h1 {
  margin-top: 12px;
  font-family: "Rubik";
  font-style: normal;
  font-weight: 500;
  font-size: 18px;
  line-height: 25px;
  text-align: center;
  color: #ffffff;
}
.grid__items__big {
  padding: 70px 30px;
}
@media (max-width: 1171px) {
  .grid__items__big,
  .items5,
  .items4,
  .items3,
  .items2,
  .items1 {
    padding: 60px 20px;
  }
}
@media (max-width: 1047px) {
  .grid__items__big,
  .items5,
  .items4,
  .items3,
  .items2,
  .items1 {
    padding: 50px 15px;
  }
  .grid__items img {
    width: 150px;
  }
}
@media (max-width: 959px) {
  .grid__items__big,
  .items5,
  .items4,
  .items3,
  .items2,
  .items1 {
    padding: 35px 10px;
  }
  .grid__items img {
    width: 130px;
  }
  .grid__items h1 {
    margin-top: 12px;
    font-family: "Rubik";
    font-style: normal;
    font-weight: 500;
    font-size: 15px;
    line-height: 20px;
    text-align: center;
    color: #ffffff;
  }
  .texts__div {
    margin-top: 50px;
  }
}

@media (max-width: 875px) {
  .Grid__content {
    margin-top: 40px;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(2, 1fr);
    gap: 20px;
  }
  .items5,
  .items4,
  .items3,
  .items2,
  .items1 {
    grid-area: initial;
  }
}
@media (max-width: 875px) {
  .Grid__content {
    margin-top: 40px;
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    grid-template-rows: repeat(1, 1fr);
    gap: 20px;
  }
  .texts__div h1 {
    font-size: 30px;
    line-height: 40px;
  }
  .texts__div h2 {
    font-size: 15px;
    line-height: 20px;
  }
}
</style>