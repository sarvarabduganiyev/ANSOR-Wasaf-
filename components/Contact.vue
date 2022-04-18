<script>
export default {};
</script>
<template>
  <section id="contact">
    <div class="max__w">
      <div class="contact__inner">
        <div class="grid__div">
          <div>
            <div class="green__box flex">
              <img
                class="green__logo__img"
                src="../img/loggo.png"
                alt="loggo"
              />
              <img
                class="green__arrow__img"
                src="../img/arrow2.png"
                alt="arrow2"
              />
            </div>
            <div class="contact__us">
              <h1>Contact Us</h1>
              <p>
                We give you exact quote before starting your project, and we
                stick to it!
              </p>
            </div>
          </div>
          <div class="form__div">
            <form class="form__contact">
              <label>Your name</label>
              <input type="text" class="inputName" />
              <label class="number__label">Your phone number</label>
              <input type="number" class="inputNumber" />
              <label class="area__label">Text</label>
              <textarea class="textArea"></textarea>
              <button class="send__btn">Send</button>
            </form>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
.grid__div {
  margin-top: 120px;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 42px;
}
.green__arrow__img {
  width: 240px;
}
.contact__us h1 {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 600;
  font-size: 40px;
  line-height: 50px;
  color: #2d3331;
}
.contact__us p {
  width: 430px;
  font-family: "Rubik";
  font-style: normal;
  font-weight: 300;
  font-size: 20px;
  line-height: 30px;
  color: #b4b4b4;
}
.form__contact {
  border: 2px solid #f1f1f1;
  border-radius: 32px;
  padding: 40px;
  width: 430px;
}
.inputName,
.inputNumber,
.textArea {
  background: #f2f2f2;
  border-radius: 8px;
  display: block;
  width: 100%;
  margin-top: 8px;
}
.inputName,
.inputNumber {
  padding: 10px;
}
.textArea {
  padding: 10px 12px 37px 12px;
  resize: none;
}
.inputName:focus,
.inputNumber:focus,
.textArea:focus {
  outline: none;
}
.textArea {
  background: #f2f2f2;
  border-radius: 8px;
}
label {
  font-family: "Rubik";
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 20px;
  color: #2d3331;
  display: block;
}
.area__label,
.number__label {
  margin-top: 22px;
}
.send__btn {
  margin-top: 30px;
  padding: 15px 70px;
  background: #3db079;
  border-radius: 8px;
  font-family: "Montserrat";
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 24px;
  color: #ffffff;
  border: 1px solid #3db079;
  transition: 0.2s ease;
}
.send__btn:hover {
  background: white;
  color: #3db079;
}
@media (max-width: 1216px) {
  .grid__div {
    margin-top: 120px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
}
@media (max-width: 1124px) {
  .green__arrow__img {
    width: 200px;
  }
  .form__contact {
    border: 2px solid #f1f1f1;
    border-radius: 32px;
    padding: 30px;
    width: 350px;
  }
  .send__btn {
    margin-top: 25px;
    padding: 10px 50px;
    border-radius: 6px;
    font-size: 14px;
    line-height: 22px;
  }
}
@media (max-width: 1024px) {
  .green__arrow__img {
    display: none;
  }
}
@media (max-width: 968px) {
  .grid__div {
    margin-top: 120px;
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    gap: 40px;
  }
  .form__div {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .contact__us p {
    width: initial;
    font-size: 17px;
    line-height: 25px;
  }
  .contact__us h1 {
    font-size: 34px;
    line-height: 40px;
  }
  .contact__inner {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .green__arrow__img {
    display: block;
    transform: rotate(100deg);
  }
  .contact__us h1 {
    text-align: center;
  }
  .contact__us p {
    text-align: center;
  }
}
@media (max-width: 750px) {
  .green__box {
    display: none;
  }
}
@media (max-width: 444px) {
  .form__contact {
    width: 270px;
    border: 2px solid #f1f1f1;
    border-radius: 20px;
    padding: 20px;
  }
  .inputName,
  .inputNumber {
    padding: 7px;
  }
  .textArea {
    padding: 7px 7px 35px 7px;
  }
  .send__btn {
    margin-top: 20px;
    padding: 10px 40px;
    border-radius: 4px;
    font-size: 12px;
    line-height: 20px;
  }
  .area__label,
  .number__label {
    margin-top: 15px;
  }
}
</style>