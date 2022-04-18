<script>
import Contact from "../components/Contact.vue";
import Five from "../components/Five.vue";
import Footer from "../components/Footer.vue";
import Four from "../components/Four.vue";
import Six from "../components/Six.vue";
import Three from "../components/Three.vue";
import Two from "../components/Two.vue";
import Tutorial from "../components/Tutorial.vue";
export default {
  components: { Tutorial, Two, Three, Four, Five, Six, Contact, Footer },
  name: "IndexPage",
};
</script>
<template>
  <div>
    <Tutorial />
    <Two />
    <Three />
    <Four />
    <Five />
    <Six />
    <Contact />
    <Footer />
  </div>
</template>
<style src="../assets/css/base.css">
</style>>

