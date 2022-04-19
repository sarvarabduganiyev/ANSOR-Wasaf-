<script>
import gsap from "gsap";

export default {
  components: {
    gsap,
  },
  mounted() {
    const items1 = document.querySelector(".numberCard__span");
    const items2 = document.querySelector(".numberCard__span2");
    const items3 = document.querySelector(".numberCard__span3");
    const items4 = document.querySelector(".numberCard__span4");
  
      gsap.from(items1, {
        textContent: 0,
        duration: 3,
        snap: { textContent: 1 },
      });
      gsap.from(items2, {
        textContent: 0,
        duration: 6,
        snap: { textContent: 1 },
      });
      gsap.from(items3, {
        textContent: 0,
        duration: 6,
        snap: { textContent: 1 },
      });
      gsap.from(items4, {
        textContent: 0,
        duration: 6,
        snap: { textContent: 1 },
      });
    }
  };
</script>
<template>
  <section>
    <div class="bg__green">
      <div class="max__w">
        <div class="texts__box">
          <h1>We create digital products</h1>
          <h3>
            We are a very experienced web & mobile app development team We are a
            very experienced web & mobile app development team
          </h3>
        </div>
        <div class="numberCard__box">
          <div class="numberCard">
            <h1><span class="numberCard__span">12</span>+</h1>
            <h2>Years of custom software development</h2>
          </div>
          <div class="numberCard">
            <h1><span class="numberCard__span2">12</span>+</h1>
            <h2>Years of app development experience</h2>
          </div>
          <div class="numberCard">
            <h1><span class="numberCard__span3">97</span>%</h1>
            <h2>of our team is hard core developers</h2>
          </div>
          <div class="numberCard">
            <h1 span class="numberCard__span4">20</h1>
            <h2>of our team is hard core developers</h2>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
.bg__green {
  margin-top: 70px;
  padding: 50px 0px 111px 0px;
  background-color: #163828;
}
.texts__box h1 {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 600;
  font-size: 40px;
  line-height: 160%;
  color: #ffffff;
  text-align: center;
}
.texts__box h3 {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 300;
  font-size: 20px;
  line-height: 160%;
  text-align: center;
  color: #c0c2c1;
  margin: 0px 250px;
}
.numberCard__box {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 50px;
  margin-top: 50px;
}
.numberCard {
  padding: 25px 40px;
  background: linear-gradient(338.57deg, #28a472 1.17%, #65c785 91.77%);
  border-radius: 16px;
}
.numberCard__box h1 {
  font-family: "Space Grotesk";
  font-style: normal;
  font-weight: 700;
  font-size: 65px;
  line-height: 102px;
  text-align: center;
  color: #ffffff;
}
.numberCard__box h2 {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 24px;
  color: #c5e7d7;
  text-align: center;
}
@media (max-width: 1149px) {
  .texts__box h3 {
    margin: 0px 150px;
  }
  .numberCard {
    padding: 10px 20px;
  }
}
@media (max-width: 1057px) {
  .texts__box h3 {
    font-size: 20px;
    line-height: 160%;
    margin: 0px 50px;
  }
  .numberCard__box h1 {
    font-size: 50px;
    line-height: 70px;
  }
  .numberCard__box h2 {
    font-size: 13px;
    line-height: 20px;
  }
}
@media (max-width: 877px) {
  .numberCard__box {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 50px;
    margin-top: 50px;
  }
}
@media (max-width: 877px) {
  .numberCard__box {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 20px;
    margin-top: 50px;
  }
  .texts__box h3 {
    margin: 0px;
    font-size: 15px;
    line-height: 160%;
  }

  .texts__box h1 {
    font-size: 30px;
    line-height: 160%;
  }
}
@media (max-width: 437px) {
  .numberCard__box {
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    gap: 20px;
    margin-top: 50px;
  }
  .texts__box h3 {
    margin: 0px;
  }
}
</style>