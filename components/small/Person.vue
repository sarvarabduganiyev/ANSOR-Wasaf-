<script>
export default {};
</script>
<template>
  <div>
    <div class="relative imgBox">
      <img
        class="absolute w-full h-full object-cover"
        src="../../img/person.png"
        alt="car"
      />
    </div>
    <div class="text__Box">
      <h1>Muhammad Xalil</h1>
      <h2>CEO</h2>
    </div>
  </div>
</template>


<style scoped>
.imgBox {
  height: 280px;
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
</style>