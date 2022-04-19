<script>
import Person from "./small/Person.vue";

export default {
  components: { Person },
  data() {
    return {
      openModal: false,
    };
  },
  methods: {
    modalFunction() {
      this.openModal = !this.openModal;
      if (this.openModal) {
        document.querySelector("body").style.overflow = "hidden";
      } else {
        document.querySelector("body").style.overflow = "initial";
      }
    },
  },
};
</script>
<template>
  <section id="about" class="max__w">
    <div>
      <div>
        <h1 class="text-center about__">About Our team</h1>
        <h3 class="text-center we__Are">
          We are a very experienced web & mobile app development team We are a
          very experienced web & mobile app development team
        </h3>
      </div>
      <div class="grid__Box">
        <Person />
        <Person />
        <Person />
        <Person />
        <Person />
      </div>
      <div class="flex flex-col justify-center items-center">
        <div class="flex img__box justify-center items-center">
          <img
            @click="modalFunction"
            class="play___img"
            src="../img/play.png"
            alt="play"
          />
          <img class="arrow___img" src="../img/arrow.png" alt="arrow" />
        </div>
      </div>
      <div
        :style="[openModal ? { display: 'block' } : { display: 'none' }]"
        id="overlay"
      >
        <div id="modal" class="bg-white">
          <div class="flex flex-col items-end">
            <button
              class="mt-3 mr-3"
              @click="modalFunction"
              id="close-modal-btn"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="h-8 w-8"
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
          </div>
          <div>
            <h1 class="text-center text-2xl text-gray-800 font-semibold">
              Video About Out Team
            </h1>
            <div
              class="
                flex
                modals__iframe__box
                flex-col
                justify-center
                items-center
                m-5
              "
            >
              <iframe width="100%" src="https://www.youtube.com/embed/tgbNymZ7vqY"> </iframe>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
#overlay {
  display: none;
  position: fixed;
  top: 0;
  right: 0;
  left: 0;
  bottom: 0;
  z-index: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  transition: 0.3s ease;
  background: rgba(7, 7, 7, 0.7);
}
#modal {
  margin: 0 auto;
  position: absolute;
  top: 20px;
  left: 20px;
  bottom: 20px;
  right: 20px;
  animation: shake 0.82s cubic-bezier(0.36, 0.07, 0.19, 0.97) both;
  transform: translate3d(0, 0, 0);
}
@keyframes shake {
  10%,
  90% {
    transform: translate3d(-3px, 0, 0);
  }

  20%,
  80% {
    transform: translate3d(5px, 0, 0);
  }

  30%,
  50%,
  70% {
    transform: translate3d(-10px, 0, 0);
  }

  40%,
  60% {
    transform: translate3d(10px, 0, 0);
  }
}
.grid__Box {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  gap: 15px;
  margin-top: 40px;
}
.modals__iframe__box iframe {
  height: 450px;
}
.play___img {
  cursor: pointer;
}
.arrow___img {
  /* margin-left: 18px; */
  margin: 40px 0px 0px 18px;
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